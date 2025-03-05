# Midterm Google Contacts

This project is a Spring Boot application that integrates with Google Contacts using OAuth2 for authentication.

## Setup

### Prerequisites

- Java 17 or higher
- Maven
- A Google Cloud project with OAuth2 credentials

### Instructions

1. **Clone the repository**:
   ```sh
   git clone https://github.com/your-username/Midterm-GoogleContacts.git
   cd Midterm-GoogleContacts
   ```

2. **Download the OAuth2 credentials JSON file**:
   - Go to the Google Cloud Console.
   - Navigate to the "Credentials" page.
   - Download the JSON file for your OAuth2 client ID.

3. **Extract the client ID and secret from the JSON file**:
   - Open the downloaded JSON file.
   - Note the `client_id` and `client_secret` values.

4. **Create a `.env` file in the project root**:
   - In the root directory of the project, create a file named `.env`.
   - Add the following content to the `.env` file:
     ```env
     GOOGLE_CLIENT_ID=your-client-id
     GOOGLE_CLIENT_SECRET=your-client-secret
     ```
   - Replace `your-client-id` and `your-client-secret` with the actual values from the JSON file.

5. **Build and run the application**:
   ```sh
   mvn clean install
   mvn spring-boot:run
   ```

6. **Access the application**:
   - Open your browser and go to `http://localhost:8080`.
   - Follow the authentication flow to grant access to your Google Contacts.

