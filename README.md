# Automated Vacation Email Sender Project

## Description

This project automates sending out email notifications to your contacts while you're on vacation. Leveraging Node.js and the Google Gmail API, it offers the following features:

**Features:**

1. **Automatic email sending:** Based on pre-defined vacation dates, the project automatically sends notifications to your mailing list.
2. **Personalized communication:** Customize email content with a personalized message and vacation details.
3. **Label handling:** Define specific labels in Gmail to identify applicable emails and only respond to those while out of office.
4. **Reply logic (optional):** Implement replying to certain emails with pre-composed responses, further automating communication.

**Components:**

1. **Node.js application:** Built using Express for creating server-side APIs and integrating with the Google Gmail API.
2. **Google Gmail API:** Provides access to manage your Gmail account and send emails programmatically.
3. **.env file:** Stores sensitive information like API keys and email credentials securely.
4. **Scheduler (optional):** Utilizes node-schedule to automatically trigger email sending on chosen vacation dates.

**Benefits:**

- **Efficiency:** Saves time and effort by automatically sending notifications instead of manually composing and sending emails before and after your vacation.
- **Professionalism:** Provides a professional, organized way to inform your contacts about your absence.
- **Peace of mind:** Ensures everyone who needs to know is informed while you're away.

**Optional Enhancements that can be tried:**

- **Integrate with calendar:** Automatically populate vacation dates from your calendar for a smoother workflow.
- **Dynamic content:** Customize content based on sender or email content for more personalized responses.
- **Tracking and metrics:** Implement email delivery tracking and analytics for insights into communication effectiveness.

**Other possible improvements**
**Enhanced logging :**

- Provide more detailed error messages, including specific thread IDs or message IDs for easier debugging.
  **Informative error messages:**
- Include user-friendly error messages when replying fails, potentially suggesting troubleshooting steps.
  **Retries or fallbacks:**
- Implement retry mechanisms for transient errors or consider alternative actions (e.g., logging errors to a file for later review).

## Features and Customization:

- **Flexible trigger conditions:** Allow users to customize the criteria for sending automated replies (e.g., based on keywords, senders, content, or other parameters).
- **Personalized email content:** Enable dynamic generation of reply content based on user input or data from external sources.
- **User-friendly configuration:** Provide an intuitive interface for users to configure reply settings, triggers, and content.

## Code Structure:

- **Modularization:** Refactor code into smaller, focused functions for better readability and maintainability.
- **Asynchronous operations:** Use promises or async/await syntax for smoother handling of asynchronous tasks.
- **Environment variables:** Consider using environment variables for configuration settings (e.g., label names, subject lines) to enhance flexibility and avoid hardcoding values.

## Setup Instructions

**Prerequisites:**

Node.js and npm (or yarn) installed on your system.

1. **Clone the repository:**

```bash
git clone https://github.com/himanshupatel457/Gmail-auto-replier.git
```

2. **Navigate to the project directory:**

   ```bash
   cd Gmail-auto-replier
   ```

3. **Install the required dependencies:**

   ```bash
   npm install
   ```

## Configuration

1. In your project's root directory, locate the `keys.env` file.
2. Create a copy of this file and name it `keys.env`. This new file will hold your sensitive information.
3. Open the `.env` file in a text editor and replace the placeholder values with your actual credentials and details:

   ```env
   PORT = 3000 // Replace with your desired port number
   GOOGLE_CLIENT_ID = YOUR_GOOGLE_CLIENT_ID
   GOOGLE_CLIENT_SECRET = YOUR_GOOGLE_CLIENT_SECRET
   REDIRECT_URI = https://developers.google.com/oauthplayground // Or your specific redirect URI
   REFRESH_TOKEN = YOUR_REFRESH_TOKEN
   LABELNAME = Vacation // Replace with the label you want to monitor
   SUBJECT = I'm currently on vacation // Replace with your desired email subject
   ```

   **Explanation of variables:**

   - **PORT:** The port number where your Node.js application will listen for incoming requests.
   - **GOOGLE_CLIENT_ID and GOOGLE_CLIENT_SECRET:** Credentials obtained from the Google Cloud Platform to access the Gmail API.
   - **REDIRECT_URI:** The URI that users will be redirected to after authorization with Google.
   - **REFRESH_TOKEN:** A long-lived token used to authenticate with the Gmail API without requiring user interaction each time.
   - **LABELNAME:** The name of the Gmail label that you want to filter emails for.
   - **SUBJECT:** The subject line to be used for the automated vacation emails.

## Run the Application

Execute the following command to start the application:

```bash
npm start
```

## Libraries and Technologies

### Dependencies:

- **dotenv (^16.3.1):** Loads environment variables from a .env file for secure configuration.
- **express (^4.18.2):** Node.js web application framework for building server-side APIs and services.
- **googleapis (^129.0.0):** Node.js client library for interacting with Google APIs.
- **node-schedule (^2.1.1):** Library for scheduling tasks in Node.js applications.

### Additional Information:

- **Programming language:** JavaScript (Node.js)
- **Version control:** Git
- **Other relevant technologies or services (if applicable):**

## Additional Notes

## Contact

```
contact : himanshupatel457@gmail.com
```
