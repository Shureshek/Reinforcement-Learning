# Tabular Q-Learning with Softmax Policy: Experiments on Classic RL Environments
**Цель проекта** — реализовать tabular Q-learning с softmax-policy с нуля и исследовать его поведение на средах с дискретным и непрерывным пространством состояний, а также сравнить с Expected SARSA в условиях принудительного исследования.


### Реализация
- Tabular Q-learning
- Softmax policy с температурой
- Тестирование работоспособности на Taxi и CartPole с дескретизацией
- Expected SARSA для сравнения
- Discretization wrapper для continuous state spaces

### Ключевые наблюдения
- Softmax policy позволяет контролировать баланс exploration-exploitation
- Слишком тонкая дискретизация CartPole приводит к медленной сходимости
- На удивление Q-learning в CliffWalking демонстрирует более безопасное поведение чем SARSA. Требуется тестирование в более сложных средах.
