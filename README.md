# Contact Manager Application

The **Contact Manager** is a simple Python application designed to manage contacts in a PostgreSQL database using the `psycopg2` library for database interactions and the `PySimpleGUI` library for creating a graphical user interface (GUI). This application allows users to insert, delete, view, and search for contacts in the database.

## Getting Started

1. **Prerequisites**: Ensure you have Python and the required libraries (`psycopg2` and `PySimpleGUI`) installed.

   You can install the required libraries using the following commands:

   ```bash
   pip install psycopg2
   pip install PySimpleGUI
   ```

2. **Database Setup**: Before running the application, make sure you have a PostgreSQL database set up with the appropriate credentials. Update the database connection parameters (database name, user, password, host, and port) in the code:

   ```python
   mydb = psycopg2.connect(database="postgres", user="postgres", password="YOUR_PASSWORD", host="localhost", port="5432")
   ```

3. **Running the Application**: Execute the provided Python script (`contact_manager.py`) to launch the Contact Manager application. The script will open a GUI window where you can interact with the application.

## Features

The Contact Manager application offers the following features:

### Insert Contact

- To add a new contact to the database, provide the contact's name, job, sex, and phone number in the input fields and click the "Insert Contact" button. The contact will be added to the database, and the updated contact list will be displayed in the output area.

### Delete Contact

- To delete a contact, enter the contact's name in the input field and click the "Delete Contact" button. The specified contact will be deleted from the database, and the contact list will be updated in the output area.

### Show Contact

- Click the "Show Contact" button to display a list of all contacts stored in the database. The contacts will be sorted by name in ascending order, and the list will be shown in the output area.

### Search Contact by Name

- To search for a specific contact by name, enter the name in the input field and click the "Search Contact by Name" button. The details of the matching contact will be displayed in the output area.

## User Interface

The application's GUI is built using the `PySimpleGUI` library, providing a user-friendly interface for interacting with the database. The GUI layout includes input fields for contact details and buttons for different actions.

## Troubleshooting

- If you encounter any issues connecting to the database, ensure that the PostgreSQL server is running and accessible using the provided connection parameters.

- For any errors or unexpected behavior, refer to the terminal/console output for error messages and stack traces.

## Contributions and Feedback

This Contact Manager application is a basic example and can be further enhanced with additional features and error handling. If you would like to contribute to the project or provide feedback, feel free to open an issue or submit a pull request on the [GitHub repository](https://github.com/yourusername/contact-manager).

## License

This project is licensed under the [MIT License](LICENSE), allowing you to use, modify, and distribute the code as needed.

---

Thank you for using the Contact Manager application! If you have any questions or need assistance, please don't hesitate to reach out to us.
