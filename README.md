# Django CRUD Project

This is a simple Django CRUD (Create, Read, Update, Delete) project that allows you to manage a list of employees. The project includes views for listing, adding, updating, and deleting employee records.

## Getting Started

Follow these instructions to set up and run the project locally on your machine.

### Prerequisites

Make sure you have the following installed:

- Python (version 3.x)
- Django (version 3.x)

### Installation

1. Clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/django-crud-project.git
    ```

2. Navigate to the project directory:

    ```bash
    cd django-crud-project
    ```

3. Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. Apply migrations to create the necessary database tables:

    ```bash
    python manage.py migrate
    ```

2. Run the development server:

    ```bash
    python manage.py runserver
    ```

3. Access the application in your web browser at [http://localhost:8000/employee/list/](http://localhost:8000/employee/list/).

4. ### Database Configuration

Update the `DATABASES` configuration in `settings.py` as follows:

```python
# settings.py

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'employeedb',
        'USER': 'root',
        'PASSWORD': '',
        'HOST': 'localhost',
        'PORT': '3310',
    }
}
```

## Features

- **Employee List:** View a list of all employees.

- **Add Employee:** Add a new employee to the list.

- **Update Employee:** Edit information for an existing employee.

- **Delete Employee:** Remove an employee from the list.

## Project Structure

- **views.py:** Contains views for listing, adding, updating, and deleting employees.

- **forms.py:** Defines the form used for employee data.

- **models.py:** Describes the Employee model.

- **employee_register/employee_list.html:** Template for displaying the list of employees.

- **employee_register/employee_form.html:** Template for the employee form.

## Contributing

Feel free to contribute to the project by opening issues or submitting pull requests.

