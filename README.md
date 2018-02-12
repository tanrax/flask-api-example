### Microframework Web

- **Flask**

### Base de datos

- **Flask-SQLAlchemy**: ORM
- **Flask-Migrate**: Añade herramientas para gestionar nuestra base de datos.
- **Flask-Script**: Creación de comandos personalizados
- **Faker**: Generador de información falsa

### API Rest

- **Flask-restplus**: Nos ayuda con las peticiones y autodocumentación
- **Flask-JWT**: Identificación básica.
- **Flask-marshmallow**: Convertirá los objetos ORM en JSON.

### Herramientas de desarrollo

- **httpie**: Cliente de API Rest para pruebas.
- **python-dotenv**: Implementación de un archivo de configuración.

### Instalación

```bash
pipenv install flask Flask-SQLAlchemy Flask-Migrate Flask-script Faker 
pipenv run python3 models.py db init
pipenv run python3 models.py db migrate
pipenv run python3 models.py db upgrade
pipenv run python3 fake_data.py
```

### Ejecución

```bash
pipenv run python3 app.py
```

## Peticiones

### GET

```bash
http GET localhost:5000/api/v1/user
```

```bash
http GET localhost:5000/api/v1/user/{id}
```

```bash
http GET localhost:5000/api/v1/notice
```

```bash
http GET localhost:5000/api/v1/notice/{id}
```

```bash
http GET localhost:5000/api/v1/notice/{id}/comments
```

### POST

```bash
http POST localhost:5000/api/v1/notice
```

```bash
http POST localhost:5000/api/v1/notice/{id}/comments
```

### PATCH

```bash
http PATCH localhost:5000/api/v1/notice/{id}
```

### DELETE

```bash
http DELETE localhost:5000/api/v1/notice/{id}
```
