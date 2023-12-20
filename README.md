# flask
# Flask Hello World API

Це простий приклад проекту на основі Flask, який надає API з однією адресою.

## Вимоги

Перед розгортанням проекту переконайтеся, що ви маєте наступні компоненти встановлені на вашому комп'ютері:

- Python 3.8 (або вище)
- Віртуальне середовище (рекомендовано)

## Розгортання

Слідуйте цим крокам для розгортання проекту:

1. **Клонуйте репозиторій на свій комп'ютер:**

   ```bash
   git clone https://github.com/obibi11/flask.git
   cd flask
   
2. Інсталюйте Python 3.8 з використанням pyenv (якщо він ще не встановлений):

   ```bash
   pyenv install 3.8.10

3. Створіть та активуйте віртуальне середовище (опціонально, але рекомендовано):

   ```bash
   python -m venv venv
   source venv/bin/activate  # Для Linux/macOS
   .\venv\Scripts\activate  # Для Windows

4. Встановіть необхідні залежності:

   ```bash
   pip install -r requirements.txt

5. Запустіть проект:

   ```bash
    python app.py

6. Відкрийте ваш веб-браузер та перейдіть за посиланням

    ```bash
     http://localhost:8080/api/v1/hello-world-22

## Використання

Цей проект надає одну адресу API:

/api/v1/hello-world-{22} - повертає текст Hello World {22} з HTTP статус кодом 200.


## Розгортання на сервері

Якщо ви бажаєте розгорнути цей проект на віддаленому сервері, ось загальні кроки, які потрібно виконати:

1. Забезпечте сервер з встановленим Python 3.8 та можливістю доступу до інтернету.
2. Клонуйте ваш репозиторій на сервер:
   
    ```bash
   git clone https://github.com/obibi11/flask.git
   cd flask
3. Створіть та активуйте віртуальне середовище:

    ```bash
    python -m venv venv
    source venv/bin/activate  # Для Linux/macOS
    .\venv\Scripts\activate  # Для Windows

4. Запустіть проект, скориставшись WSGI-сервером, наприклад Gunicorn:

    ```bash
    gunicorn -w 4 -b 0.0.0.0:8080 app:

5. Пропустіть трафік до вашого серверу через порт 8080. Тепер ваш API доступний за посиланням

      ```bash
      http://your_server_ip:8080/api/v1/hello-world-22.
