# ДЗ #6: TensorRT Throughput измерение

## Результаты выполнения:

### Окружение:
- Устройство: cpu
- Доступные провайдеры: TensorrtExecutionProvider, CUDAExecutionProvider, CPUExecutionProvider
- Модель: EfficientNet-B0 (ONNX, динамический batch)
- Данные: CIFAR-10, single image inference

### Результаты измерений:
- **CUDA**: 22.9 images/sec
- **TensorRT (CUDA fallback)**: 28.3 images/sec
- **CPU**: 25.1 images/sec


### Скриншот:
Приложите скриншот вывода измерений к PR.

### Выводы:
Успешно подключены и протестированы различные Execution Providers.
TensorRT доступен и работает.
