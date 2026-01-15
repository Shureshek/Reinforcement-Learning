# REINFORCE Policy Gradient для задачи CartPole

[![Python 3.9+](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/)
[![PyTorch](https://img.shields.io/badge/PyTorch-2.0+-red.svg)](https://pytorch.org/)
[![Gymnasium](https://img.shields.io/badge/Gymnasium-0.29+-green.svg)](https://gymnasium.farama.org/)

Реализация алгоритма REINFORCE (Policy Gradient) с обучением с подкреплением для решения задачи CartPole-v1 из библиотеки Gymnasium.

## Цель проекта

Практическая реализация и понимание:
- Алгоритма REINFORCE (Policy Gradient)
- Методов обучения с подкреплением без модели
- Работы с нейронными сетями в PyTorch для RL
- Визуализации результатов обучения

## Теоретическая основа

REINFORCE — это алгоритм обучения с подкреплением, который оптимизирует политику напрямую, используя градиент ожидаемого вознаграждения:

∇θ J(θ) ≈ (1/N) ∑ ∇θ log πθ(a|s) * G(s,a)

где:
- πθ(a|s) — политика (вероятность выбора действия)
- G(s,a) — дисконтированное совокупное вознаграждение
- θ — параметры нейронной сети
