# ДЗ #4: Early Stopping и Checkpoints

## Результаты выполнения

### Параметры:
- Модель: EfficientNet-B0 (предобученная)
- Обучение: fine-tuning только последнего слоя
- Данные: CIFAR-10 (уменьшенная выборка)
- Устройство: cpu
- Early Stopping patience: 2
- Макс эпох: 5

### Результаты обучения:
- Обучено эпох: 5
- Лучшая точность: 0.650
- Лучшая эпоха: 4
- Время обучения: 210.2 секунд
- Размер checkpoint: 16094.2 KB

### Содержимое checkpoint.tar:
1. model_state_dict - веса модели
2. optimizer_state_dict - состояние оптимизатора
3. epoch - номер эпохи
4. accuracy - лучшая точность
5. loss - значение loss

### Файлы:
- checkpoint.tar - полный checkpoint
- docs/early_stopping_plot.png - график обучения

### Вывод:
Early Stopping успешно реализован. При достижении максимальной точности модель сохраняется в checkpoint.
Checkpoint содержит все необходимые компоненты для продолжения обучения.
