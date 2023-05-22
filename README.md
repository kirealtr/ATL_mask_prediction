# ATL_mask_prediction
Этот репозиторий посвящен проекту по курсу машинного обучения и по физике. Цель: обучить модель предсказывать маску ахроматической Талбот-литографии по заданной картине дифракции. 

## Симуляции дифракции

В ноутбуке atl_simulation.ipynb есть все функции, необходимые для получения дифракционных картин по произвольной маске. Можно посчитать как обычную саморепродукцию (ковер Талбота), так и ахроматическую (ATL). В ноутбуке cnn_with_sims.ipynb можно найти адаптацию ATL симуляции под тензор библиотеки PyTorch.

## Генерация случайных масок

Ноутбук picture_generator.ipynb использовался для создания датасета из случайных бинарных масок. Там вы можете найти примеры использования библиотеки PIL для рисования различных фигур.

## Нейронные сети

Модели сверточных нейросетей для предсказания масок и алгоритмы их обучения представлены в ноутбуках cnn.ipynb и cnn_with_sims.ipynb. При обучении для ускорения используется mixed precision training. Отличаются ноутбуки способом валидации и теста.
