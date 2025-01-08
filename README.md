
# Django Todo API

This project is a simple Todo API built using Django and the Django REST framework. The application allows users to create and manage a list of todo items with basic CRUD functionality.

## Features

- Create, read, update, and delete todo items.
- Admin interface for managing todo items.
- Unit tests for model validation.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Sam-Waithaka/Todo-API.git
   cd todo-api
   ```

2. Install the dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Apply the migrations:

   ```bash
   python manage.py migrate
   ```

4. Run the development server:

   ```bash
   python manage.py runserver
   ```

5. Access the API at `http://127.0.0.1:8000/` and the admin interface at `http://127.0.0.1:8000/admin/`.

## Model

### Todo

- `title`: A `CharField` with a maximum length of 200 characters, representing the title of the todo item.
- `body`: A `TextField` for the body or description of the todo item.

## Admin

The `Todo` model is registered in the Django admin with the `title` and `body` fields displayed in the list view.

## Testing

The project includes unit tests for the `Todo` model:

- Validates the content of the `title` and `body` fields.

Run the tests using:

```bash
python manage.py test
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or report issues.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
