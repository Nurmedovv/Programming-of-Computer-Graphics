# Лабораторные работы по компьютерной графике

Репозиторий с выполненными лабораторными работами по курсу компьютерной графики.  
**Вариант 8**: Визуализация буквы "N" в 3D.

## 🛠 Стек технологий

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" height="30"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" height="30"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" height="30"/>
  <img src="https://img.shields.io/badge/Canvas_API-2C3E50?style=for-the-badge&logo=html5&logoColor=white" alt="Canvas API" height="30"/>
  <img src="https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white" alt="WebGL" height="30"/>
  <img src="https://img.shields.io/badge/ExifJS-FF6600?style=for-the-badge&logo=javascript&logoColor=white" alt="ExifJS" height="30"/>
  <img src="https://img.shields.io/badge/Piexif-2C8EBB?style=for-the-badge&logo=javascript&logoColor=white" alt="Piexif" height="30"/>
</p>

## 📚 Список работ

| № | Название | Описание |
|---|----------|----------|
| **1** | Image Metadata Analyzer | Анализ метаданных изображений (JPG, PNG, GIF, BMP, TIFF, WEBP). Извлечение EXIF-данных, матрицы квантования JPEG, визуализация гистограмм. |
| **2** | Редактор изображений | Интерактивная обработка изображений: яркость/контраст, гистограмма, пороговая обработка, морфологические операции (дилатация/эрозия), детекторы границ (Собель, Кэнни, Харрис, FAST). |
| **3** | Базовые растровые алгоритмы | Визуализация алгоритмов растеризации: пошаговый, ЦДА, Брезенхема (отрезок и окружность), кривые Безье (Кастлжо), сглаживание линий (алгоритм Ву). **Пошаговый режим** для обучения. |
| **4** | Алгоритмы отсечения | Отсечение отрезков и многоугольников прямоугольным окном: алгоритм средней точки и Сазерленда-Ходжмена. Загрузка данных из файла, масштабирование/панорамирование. |
| **5** | Конвертер цветовых моделей | Двусторонняя конвертация между моделями RGB ↔ HSV ↔ XYZ ↔ LAB. Превью цвета, история операций, синхронизация ползунков и числовых полей. |
| **6** | 3D Визуализация буквы "N" | Трехмерная модель буквы "N" с управлением: масштаб, поворот по трём осям (X, Y, Z), перенос. Матричные преобразования, проекции на плоскости XY, XZ, YZ. Управление мышью и автоповорот. |

## 🚀 Как запустить

### Вариант 1: Локальный запуск

1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/your-username/computer-graphics-labs.git
   cd computer-graphics-labs
   ```

2. **Откройте нужную лабораторную работу:**
   - Просто откройте `index.html` в любой из папок в браузере
   - Рекомендуется использовать Live Server в VS Code

### Вариант 2: Запуск через Live Server (рекомендуется)

1. **Установите расширение** "Live Server" в VS Code
2. **Откройте папку** с проектом в VS Code
3. **Кликните правой кнопкой** на `index.html`
4. **Выберите** "Open with Live Server"

### Вариант 3: Запуск всех работ через общий сервер

```bash
npx serve .
```

После запуска сервер будет доступен по адресу `http://localhost:3000` (или другому порту).

## 📁 Структура репозитория

```
computer-graphics-labs/
├── lab1-image-metadata-analyzer/
│   └── index.html
├── lab2-image-editor/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── lab3-raster-algorithms/
│   ├── index.html
│   └── script.js
├── lab4-clipping-algorithms/
│   └── index.html
├── lab5-color-converter/
│   ├── index.html
│   ├── style.css
│   └── script.js
├── lab6-3d-letter-n/
│   └── index.html
└── README.md
```

## 🎯 Особенности реализации

### Лабораторная работа №1
- Поддержка до 100,000 файлов одновременно
- Drag-and-drop загрузка
- EXIF-анализ с помощью библиотеки piexifjs
- Визуализация матрицы квантования JPEG
- Экспорт результатов в CSV

### Лабораторная работа №2
- Мгновенное применение фильтров (real-time)
- Детекторы границ: Собель, Прюитт, Лапласиан, Кэнни, Харрис, FAST
- Морфологические операции: дилатация, эрозия, открытие, закрытие
- Адаптивная и глобальная пороговая обработка (метод Оцу)
- Визуализация гистограмм RGB с математической статистикой

### Лабораторная работа №3
- Пошаговый режим с отображением вычислений
- Система координат с центром в середине canvas
- Клик по сетке для ввода координат
- Регулировка размера сетки (10-50px)

### Лабораторная работа №4
- Загрузка данных из текстового файла
- Встроенный пример для тестирования
- Масштабирование и панорамирование
- Две проекции: ортографическая для 2D, перспективная для 3D

### Лабораторная работа №5
- Точность до 5 знаков после запятой (HSV)
- Автоматическая синхронизация всех моделей
- История последних 10 цветов
- Прямое преобразование через матрицы XYZ (не через промежуточные модели)

### Лабораторная работа №6
- Вращение модели мышью (drag-and-drop)
- Отображение полной матрицы преобразования 4×4
- Три проекции (XY, XZ, YZ) в реальном времени
- Автоповорот с регулируемой скоростью

## 📊 Демонстрация алгоритмов

| Алгоритм | Лабораторная работа |
|----------|---------------------|
| EXIF-анализ | №1 |
| Линейное контрастирование | №2 |
| Выравнивание гистограммы | №2 |
| Алгоритм Оцу | №2 |
| Пошаговая растеризация | №3 |
| ЦДА | №3 |
| Брезенхема (линия/окружность) | №3 |
| Кастлжо (кривые Безье) | №3 |
| Алгоритм Ву (сглаживание) | №3 |
| Отсечение отрезков | №4 |
| Отсечение многоугольников | №4 |
| RGB → HSV → XYZ → LAB | №5 |
| Матричные 3D-преобразования | №6 |

## 👤 Автор

- **Нурмедов Азат**
- **Telegram:** @fakevv
- **Instagram:** nurmedovv
- **Email:** azatnurmedovv2554@gmail.com

*Все работы выполнены самостоятельно в соответствии с методическими указаниями.*

---

# Computer Graphics Laboratory Works

Repository with completed laboratory works for the computer graphics course.  
**Variant 8**: 3D visualization of the letter "N".

## 🛠 Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5" height="30"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3" height="30"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript" height="30"/>
  <img src="https://img.shields.io/badge/Canvas_API-2C3E50?style=for-the-badge&logo=html5&logoColor=white" alt="Canvas API" height="30"/>
  <img src="https://img.shields.io/badge/WebGL-990000?style=for-the-badge&logo=webgl&logoColor=white" alt="WebGL" height="30"/>
</p>

## 📚 List of Works

| # | Title | Description |
|---|-------|-------------|
| **1** | Image Metadata Analyzer | Image metadata analysis (JPG, PNG, GIF, BMP, TIFF, WEBP). EXIF data extraction, JPEG quantization matrix, histogram visualization. |
| **2** | Image Editor | Interactive image processing: brightness/contrast, histogram, thresholding, morphological operations, edge detectors (Sobel, Canny, Harris, FAST). |
| **3** | Raster Algorithms | Visualization of rasterization algorithms: step-by-step, DDA, Bresenham (line and circle), Bezier curves (Casteljau), Wu antialiasing. **Step-by-step mode** for learning. |
| **4** | Clipping Algorithms | Line and polygon clipping with rectangular window: midpoint algorithm and Sutherland-Hodgman algorithm. File data loading, zooming/panning. |
| **5** | Color Converter | Bidirectional conversion between RGB ↔ HSV ↔ XYZ ↔ LAB color models. Color preview, operation history, slider and input field synchronization. |
| **6** | 3D Letter "N" Visualization | 3D model of the letter "N" with controls: scale, rotation around three axes (X, Y, Z), translation. Matrix transformations, projections onto XY, XZ, YZ planes. Mouse control and auto-rotation. |

## 🚀 How to Run

### Option 1: Local Launch

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/computer-graphics-labs.git
   cd computer-graphics-labs
   ```

2. **Open the desired lab:**
   - Simply open `index.html` in any lab folder in your browser
   - Live Server in VS Code is recommended

### Option 2: Live Server (Recommended)

1. **Install** the "Live Server" extension in VS Code
2. **Open** the project folder in VS Code
3. **Right-click** on `index.html`
4. **Select** "Open with Live Server"

### Option 3: Run all labs via a common server

```bash
npx serve .
```

After starting, the server will be available at `http://localhost:3000`.

## 👤 Author

- **Azat Nurmedov**
- **Telegram:** @fakevv
- **Instagram:** nurmedovv
- **Email:** azatnurmedovv2554@gmail.com

*All works were completed independently in accordance with the methodological guidelines.*
```
