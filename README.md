# GitPractics

#Изменения требуемые в пункте 6 лаб1
```
from flask import Flask
from app.views.MainController import main_controller
from app.views.AuthController import auth_controller

app = Flask(__name__, static_url_path='', static_folder='static')

# Регистрация контроллеров
app.register_blueprint(main_controller)
app.register_blueprint(auth_controller)


if __name__ == '__main__':
    app.run(debug=True)
```