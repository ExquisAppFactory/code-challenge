<h1 align="center">
	<img alt="Discord logo" src="https://github.com/ExquisAppFactory/lightweight/blob/master/assets/monorepo.svg" height="150px" width="150px" />
</h1>

<h3 align="center">
  Light Weight App architecture
</h3>

## 📝 Project Requirement

Since Covid-19, there has been a surge in online businesses. Business owners need an easy way to send invoice to their customers.
Your starup needs to provide a service that sends invoices to customers. You will be using the microservice architecture to architect
the system, ensuring that services are available at scale.

## User Service

You can use a third party authentication service to create a user service for your application

## Invoice service

Create an Invoice service that accepts necessary information. This service can generate a pdf version of the invoice with a defined template.

## Email Service

Create a service that accepts the necessary information and sends emails. It should provide an abstraction between two different email service providers. If one of the services goes down, your service can quickly failover to a different provider without affecting your customers.

Example Email Providers:

1. SendGrid - [Simple Send Documentation](https://sendgrid.com/docs/API_Reference/Web_API/mail.html)
2. Mailgun - [Simple Send Documentation](http://documentation.mailgun.com/quickstart.html#sending-messages)
3. SparkPost - [Developer Hub](https://developers.sparkpost.com/)
4. Amazon SES - [Simple Send Documentation](http://docs.aws.amazon.com/ses/latest/APIReference/API_SendEmail.html)

All listed services are free to try and are pretty painless to sign up for, so please register your own test accounts on each.

### Technical Requirement:

- Use third party Auth to handle user authentication
- Services should be granulated and be standalone. For example I should be able to user the Invoice service without the Email or User Service
  Likewise, I should be able to use the Email service independently
- Send Invoices to Customers via the Email service
- Expose API endpoints of all the microservices

### Functional Requirement:

- Users should be able to fund their wallets by making payment online (please feel free to use a mock payment)
- Users wallet are expected to be debited when they pay for a service
- Service provide's wallet is to be credited with the service charge collected from customers

### Frontend

- You are expected to build a simple but responsive UI to consume the APIs

## 🚀 Technologies

Please feel free to use any of the technologies listed below:

### Backend

- Java Springboot
- Node.js & Express (javascript & Typescript)
- Python (Any Python stack)

### Database

- MongoDB
- MySQL
- PostGre SQL

### Messaging

- Apache Kafka
- Rabbit MQ

### Others

- Docker

### Frontend

- React
- Angular

## ✅ Accessment Criteria

- Good file structure and naming convention
- Your code must be unit tested both on the backend and frontend
- You are expected to containerize using the app `Docker`
- Application should be deployed to `AWS`
- Set up CI/CD pipelines using `Github actions`
- There should a proper `README` on your project

## 🤔 How to contribute

**Follow the steps below**

```bash
> Clone your fork and make it private

> When you are done with the work share it  with the following address

```
