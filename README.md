# Video Request Management SPA

Welcome to the Video Request Management SPA, a web application that allows users to submit and manage video requests, vote on their favorite requests, and perform various administrative actions. This project is part of the YallaCode Academy's Ramadan 2020 assessments.

## Getting Started

To get started with this project, follow the steps below:

1. **Clone the Repository:** Clone this repository to your local machine.

2. **Install Dependencies:** Navigate to the server directory and install the required dependencies:

   ```bash
   cd server
   npm install
   ```

3. **Configure MongoDB:** Set up a local MongoDB database and copy the connection URL to the required place in `server/models/mongo.config.js`.

4. **Start the Server:** Run the server using the following commands:

   ```bash
   npm start
   ```

5. **Access the Application:** Open the project in your web browser.

## Features

### Video Requests

- **Submit a Video Request:** Users can submit video requests, including details such as the topic title, description, and more.

- **View List of Requests:** All video requests are displayed in a user-friendly list below the submission form.

- **Vote Up and Down:** Users can vote up or down on each video request to show their support or disapproval.

- **Sorting Options:** Sort the video requests by "new first" (default) or "top voted first" to view requests in the desired order.

- **Search Functionality:** Easily search for video requests by entering keywords in the search box.

- **Client-Side Validation:** The form includes client-side validation for required fields and email validation. The topic title is limited to 100 characters.

### User Management

- **User Login:** Users can create accounts and log in using their email addresses.

- **Unique User Votes:** To ensure fairness, users are allowed to vote only once on each request. Votes are tracked by unique user information.

### Super User Capabilities

- Super users have special privileges that allow them to:
  - Delete requests
  - Add resolution videos
  - Change request statuses
  - Access specific styling for their capabilities
  - Filter requests by status (NEW, PLANNED, DONE)

## Technical Details

- The project is implemented using pure, modern **JavaScript** code without external libraries or utilities.
- AJAX is used to make the project behave like a Single Page Application (SPA).
- For styling, Bootstrap classes are utilized, and no additional CSS is required.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute this project according to the terms of the license.
