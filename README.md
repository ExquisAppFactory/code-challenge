<h1 align="center">
	<img alt="Discord logo" src="https://github.com/ExquisAppFactory/lightweight/blob/master/assets/monorepo.svg" height="150px" width="150px" />
</h1>

<h2 align="center">
  Invoice Management System
</h2>

### 📝 Project Requirement

Since Covid-19, there has been a surge in online businesses. Business owners need an easy way to send invoice to their customers.
Your starup needs to provide a service that sends invoices to customers. You will be using the microservice architecture to architect
the system, ensuring that services are available at scale.

### User Service

- Integrate third-party authentication for user sign-up and login (e.g., Auth0, Firebase Auth).
- Maintain user profiles with necessary details (e.g., name, email, wallet balance).

### Invoice service

- Accept and store invoice-related details from users.
- Generate a downloadable PDF version of the invoice based on a predefined template.

### Email Service

- Accept invoice details and recipient email.
- Provide an abstraction layer over multiple email service providers. If one fails, it should transparently switch to another.
- Recommended Email Providers: [SendGrid](https://sendgrid.com/docs/API_Reference/Web_API/mail.html), [Mailgun](http://documentation.mailgun.com/quickstart.html#sending-messages), [SparkPost](https://developers.sparkpost.com/), [Amazon SES](http://docs.aws.amazon.com/ses/latest/APIReference/API_SendEmail.html).

### Technical Requirement:

- Use third-party authentication for user handling.
- Each service should be independent. They should be capable of operating separately and be consumed independently.
- Expose well-documented API endpoints for all services.

### Frontend

- Develop a responsive web-based interface.
- Allow users to:
    - Register and log in.
    - Add funds to their wallets.
    - Create, view, and send invoices.
    - Track their wallet's transaction history.
    - View the status of sent emails (e.g., sent, delivered, failed).

## 🚀 Technologies

You can use any of the languange or technology listed below unless otherwise stated:

### Backend

- Java Springboot
- Node.js & Express (javascript & Typescript)
- Python (Any Python stack)

### Database

- MongoDB
- MySQL
- PostGre SQL

### Others

- Docker

### Frontend

- React
- Angular

## **Additional Suggestions:**

- Include logging to track failures or errors in the system.
- Set up CI/CD pipelines using `Github actions`
- Use containerization (e.g., Docker, Docker Compose) for services to ensure a consistent development and deployment environment.

## ✅ Accessment Criteria

1. API Design: Clear, consistent, and documented API endpoints.
2. Code Quality: Clean, maintainable, and efficient code.
3. System Design: Scalable and resilient system architecture.
4. Error Handling: Robust handling of possible failures and errors.
5. Unit tests both on the backend and frontend

## Instruction
Fork this repository
All your changes should be made in a private fork of this repository. When you're done please, please:

Share your fork with the `exquis-test` user (Settings -> Collaborators -> Add People)

Reply to the email that asked you to do this API exercise, with a link to the repository that the exquis-test user now should have access to.
