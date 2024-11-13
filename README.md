# File Hider Project (Java)

## Overview
The **File Hider Project** is a secure file management system built in Java that allows users to hide files and retrieve them when needed. It employs OTP (One-Time Password) authentication to ensure security and uses the **Model-View-Controller (MVC)** architecture for an organized and scalable design.

## Features
- **OTP Authentication**: Secure login system using OTP sent via email to authenticate users.
- **File Hiding**: Users can hide files in the system, encrypt them for security, and access them later.
- **MVC Architecture**: The application follows the MVC pattern, ensuring clean separation of concerns and maintainability.
- **File Encryption**: Encrypts hidden files to ensure unauthorized users cannot access them.

## Technologies Used
- **Java**: The main programming language for developing the application.
- **MySQL**: Used for storing user credentials and OTP verification data.
- **JavaMail API**: Used to send OTPs to users via email.
- **MVC Architecture**: Separates the application logic into Model, View, and Controller components.

## Installation

1. Clone this repository to your local machine:

    ```bash
    git clone https://github.com/harika-mini/file-hider-java.git
    ```

2. Install MySQL and create a database for user credentials and OTP.

3. Configure the database connection by editing the `db-config.properties` file with your MySQL credentials.

4. Compile the Java project using the following commands:

    ```bash
    javac -d bin src/*.java
    ```

5. Run the project:

    ```bash
    java -cp bin Main
    ```

## Usage

1. **Login**:
   - When you run the application, you’ll be prompted to enter your username.
   - An OTP will be sent to your registered email address.
   - Enter the OTP to authenticate and gain access to the file management system.

2. **Hiding Files**:
   - After authentication, you can choose to hide files by providing the file path.
   - The file will be encrypted before hiding.

3. **Accessing Hidden Files**:
   - You can retrieve a hidden file by providing the appropriate decryption key.
   
## MVC Architecture Breakdown

- **Model**: Handles the data operations (file encryption, user authentication, database interactions).
- **View**: The user interface that interacts with the user, displaying prompts for OTP verification, file hiding, and retrieval.
- **Controller**: Manages the flow between the model and the view, handling the business logic and coordinating actions (e.g., sending OTP, managing file hiding/retrieval).

## Contributing
Feel free to fork this repository and submit pull requests. Any contributions or improvements are welcome!

## License
This project is licensed under the MIT License.
