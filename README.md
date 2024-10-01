# Calculator

Это веб-калькулятор, стилизованный под калькулятор Windows, реализованный с помощью **HTML**, **CSS** и **JavaScript**. Проект включает в себя `Dockerfile` и `docker-compose.yml` для удобного развертывания приложения в **Docker** контейнере.

## 📋 Функциональность

- **Арифметические операции**: сложение, вычитание, умножение, деление.
- **Математические функции**:
  - Квадрат (`x²`)
  - Квадратный корень (`√`)
  - Экспонента (`eˣ`)
  - Натуральный логарифм (`ln`)
  - Десятичный логарифм (`log`)
- **Поддержка скобок** для группировки выражений.
- **Интерфейс**, напоминающий калькулятор Windows.

## 🚀 Запуск проекта

### Предварительные требования

- Установленный **Docker** (версия 19.03 и выше).
- Установленный **Docker Compose** (обычно включен в Docker Desktop для Windows и macOS).

### Инструкция по запуску

1. **Клонируйте репозиторий** (или скачайте архив с кодом):

   ```bash
   git clone https://github.com/your-username/calculator.git
   ```

2. **Перейдите в директорию проекта**:

   ```bash
   cd calculator
   ```

3. **Запустите приложение** с помощью Docker Compose:

   ```bash
   docker-compose up --build
   ```

   > ⚠️ **Примечание**: Флаг `--build` заставляет Docker пересобрать образ перед запуском, обеспечивая актуальность приложения.

4. **Откройте браузер** и перейдите по адресу:

   ```
   http://localhost
   ```

   Теперь вы можете пользоваться калькулятором!

## 🛑 Остановка приложения

Чтобы остановить приложение, нажмите `Ctrl+C` в терминале, где оно запущено, или выполните команду:

```bash
docker-compose down
```

## 📂 Структура проекта

- `index.html` — основной HTML-файл с разметкой и встроенными скриптами.
- `Dockerfile` — инструкция для сборки Docker-образа.
- `docker-compose.yml` — конфигурационный файл для Docker Compose.
- `README.md` — документация проекта (этот файл).

## ✨ Функциональные особенности

- **Интуитивно понятный интерфейс** с кнопками, напоминающими калькулятор Windows.
- **Отображение ошибок**: если введено некорректное выражение, на дисплее появится сообщение "Ошибка".
- **Поддержка клавиатуры**: вы можете использовать мышь или тачпад для нажатия кнопок.

## 📖 Примеры использования

- **Квадрат числа**: введите число и нажмите `x²`.
- **Квадратный корень**: нажмите `√`, введите число и закройте скобку `)`.
- **Экспонента**: нажмите `eˣ`, введите степень и закройте скобку `)`.
- **Логарифмы**:
  - Натуральный логарифм: `ln(` число `)`
  - Десятичный логарифм: `log(` число `)`

## 🛠 Возможные проблемы и их решения

- **Порт 80 уже используется**:
  - Измените порт в `docker-compose.yml`:

    ```yaml
    ports:
      - '8080:80'
    ```

  - Запустите приложение и перейдите по адресу `http://localhost:8080`.

- **Docker не установлен**:
  - Скачайте и установите Docker с официального сайта: [https://www.docker.com/get-started](https://www.docker.com/get-started)

## 📬 Обратная связь

Если у вас есть вопросы или предложения по улучшению проекта, пожалуйста, создайте [issue](https://github.com/your-username/calculator/issues) в репозитории или свяжитесь со мной по электронной почте: [your-email@example.com](mailto:your-email@example.com).

## 📝 Лицензия

Этот проект распространяется под лицензией [MIT](LICENSE).

---

Спасибо за использование этого калькулятора! 😊
