# NEXT JS BASED FEEDBACK HUB WEB APP

## Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Deployment](#deployment)
- [Authors](#authors)
- [Acknowledgements](#acknowledgements)
- [Support](#support)

## Project Description

Feedback Hub is designed to help users receive honest and anonymous feedback from their peers. Users can sign up, verify their accounts, and start receiving messages. The platform ensures privacy and security by verifying users and managing messages efficiently.

## Features

- User Authentication (Sign Up, Sign In, Verification)
- Anonymous Messaging
- Real-time Notifications
- User Profile Management
- Message Suggestions using OpenAI

## Tech Stack

**Front-end:**

- Next JS
- Redux
- ShadCN

**Back-end:**

- Next JS


**Database:**

- MongoDB
- Zod

**Authentication**

Next Auth

**API Endpoints Testing:**

- Postman


## Deployment

Hosting platform: [Varcel](https://feedback-hub-liart.vercel.app/)


## Authors

- [@Sameer Shrikhande](https://github.com/sameershrikhande)

## Acknowledgements

- [React](https://react.dev/)
- [Next JS](https://nextjs.org/)
- [ShadCN](https://mui.com/)
- [MongoDB](https://www.mongodb.com/atlas/database)
- [Zod](https://zod.dev/)
- [NextAuth](https://next-auth.js.org/)
- [Resend](https://resend.com/)


## Support

For support, contact:

- Email: sameershrikhande6@gmail.com
- LinkedIn: [Sameer Shrikhande](https://www.linkedin.com/in/sameershrikhande/)

## Contact

For any questions or feedback, please contact me at [sameershrikhande5@gmail.com](mailto:sameershrikhande6@gmail.com).

---
---
---


## Reference Notes : 📝

### Algorithm for Creating User - Signup

- Our algorithm ensures that users with an already verified email cannot register again, while allowing those who haven't verified their email to update their information. New users are created and saved with the provided details.

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
