# Feedback Hub

Feedback Hub is a platform that allows users to receive anonymous feedback and messages. It is built using Next.js and integrates with various APIs to provide a seamless user experience.

## Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contact](#contact)

## Project Description

Feedback Hub is designed to help users receive honest and anonymous feedback from their peers. Users can sign up, verify their accounts, and start receiving messages. The platform ensures privacy and security by verifying users and managing messages efficiently.

## Features

- User Authentication (Sign Up, Sign In, Verification)
- Anonymous Messaging
- Real-time Notifications
- User Profile Management
- Message Suggestions using OpenAI

## Installation

To get started with Feedback Hub, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/sameershrikhande/Feedback-Hub.git
    cd feedback-hub
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Set up environment variables:**

    Create a `.env` file in the root directory and add the necessary environment variables. Refer to `.env.example` for the required variables.

4. **Run the development server:**

    ```bash
    npm run dev
    ```

    Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Usage

### Sign Up

1. Navigate to the Sign-Up page.
2. Enter your username, email, and password.
3. Verify your email using the verification code sent to your email address.

### Sign In

1. Navigate to the Sign-In page.
2. Enter your email and password.
3. Access your dashboard to manage messages and profile settings.

### Sending Messages

1. Go to a user's profile page.
2. Enter your message in the provided text box.
3. Click "Send" to send the message anonymously.

## API Endpoints

### Authentication

- **POST /api/sign-up**: Register a new user.
- **POST /api/sign-in**: Authenticate a user.
- **POST /api/verify-code**: Verify a user's email using a verification code.

### Messages

- **POST /api/send-message**: Send an anonymous message to a user.
- **GET /api/get-messages**: Retrieve messages for a user.
- **DELETE /api/delete-message/:messageid**: Delete a specific message.

### Suggest Messages

- **POST /api/suggest-messages**: Get suggested messages using OpenAI.



## Contact

For any questions or feedback, please contact me at [sameershrikhande5@gmail.com](mailto:sameershrikhande5@gmail.com).

---

Thank you for using Feedback Hub! I hope you find it useful


---
---
---
---
---
---


## Reference Notes : 📝

### Algorithm for Creating User - Signup

- Our ensures that users with an already verified email cannot register again, while allowing those who haven't verified their email to update their information. New users are created and saved with the provided details.

```
IF existingUserByEmail EXISTS THEN
    IF existingUserByEmail.isVerified THEN
        success: false
    ELSE
        // Update and save the existing user's information
    END IF
ELSE
    // Create and save a new user with the provided details
END IF
```
