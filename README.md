📊 Приложение построения графиков температуры

Приложение предназначено для визуализации данных о температуре из текстового файла. Оно считывает данные из файла с показаниями времени, даты и трёх параметров температуры (установленная температура, зафиксированная температура 1 и 2), строит график и сохраняет его в виде изображения PNG.

Пример строки данных:
`00:09:06 05-06-2024	540	287	422`

🧰 Функционал
- 🔍 Автоматическое определение кодировки файла (включая UTF-8, UTF-16 и т.п.)
- 📈 Построение графика с тремя линиями:
  - Установленная температура (SP)
  - Зафиксированная температура 1 (PV1)
  - Зафиксированная температура 2 (PV2)
- 💾 Сохранение графика как изображение PNG с автоматически сгенерированным именем: `<имя_файла>_graph.png- `
- 🖥️ Графический интерфейс на tkinter с возможностью выбора файла через диалоговое окно

📦 Требования
Для корректной работы программы необходимо установить следующие библиотеки:
`pip install chardet matplotlib`

▶️ Запуск приложения
- Скачайте или склонируйте репозиторий.
- Убедитесь, что установлены все зависимости (см. выше).
- Запустите программу командой:
`python Temp_Trend_png_excel_graph.py`
- В открывшемся окне нажмите "Выбрать файл" и укажите текстовый файл с данными.
- Программа построит график и сохранит его в той же директории, где находится исходный файл.

![График](https://github.com/wxxxenly/temperature_analysis/blob/13a1fd80f7feb2df79b0f5c1dbbe7b3a48991f14/dist/temperature_analysis/Temp%20Trend_SP%2CPV_250507_graph.png)
