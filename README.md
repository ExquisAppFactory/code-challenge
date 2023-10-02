<h1 align="center">
	<img alt="Discord logo" src="https://github.com/ExquisAppFactory/lightweight/blob/master/assets/monorepo.svg" height="150px" width="150px" />
</h1>

<h3 align="center">
  Light Weight App Monorepo architecture
</h3>

## 👨🏻‍💻 About the project

The Light Weight app is a project which is was born out of the idea of creating a way for new consultants to have hands-on experience with day-to-day cutting edge technologies which will be needed for their consulting projects. The project is using a monorepo architecture so that it will be easier for consultants to add their contributions as a project.

## 📝 Project Requirement

MoneyPal is a fictitous marketplace system where user have offers and request for services. Users have a virtual wallet where they can credit their wallets from within the system

The goal of this mini project is to build a backend services using the microservice architecture to facilitate transfer of money from a wallet to another wallet. Note that, the said system should have a `user service`, `payment service`, `billing service`, and a `wallet service` respectively.

### Technical Requirement:

- Create a mechanism for registering and authenticating users
- There should be a way to notify service providers and customers of a transaction (email notification is preferable)
- Expose API endpoints of all the microservices

### Functional Requirement:

- Users should be able to fund their wallets by making payment online (please feel free to use a mock payment)
- Users wallet are expected to be debited when they pay for a service
- Service provide's wallet is to be credited with the service charge collected from customers

### Frontend

- You are expected to build a simple but responsive UI to consume the APIs

## 🛢 Database Schema

- User Service -> (`id`, `first_name`, `last_name`, `password`, `email`)
- Wallet Service -> (`id`, `user_id`, `balance`)
- Billing Service -> (`id`, `user_id`, `invoice_no`, `amount`, `date`, `status`)
- Payment Service -> (`id`, `paid_by`, `amount_paid`, `paid_to`, `status`, `date`)

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
- Vue

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
# Clone your fork
$ git clone https://github.com/ExquisAppFactory/lightweight.git

$ cd lightweight

$ cd packages

$ mkdir your-name

# Create a branch with your feature
$ git checkout -b your-name

# Make the commit with your changes
$ git commit -m 'feat: Your new feature'

# Send the code to your remote branch
$ git push origin your-feature
```

After your pull request is merged, you can delete your branch
