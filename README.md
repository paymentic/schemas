# Schemas

Welcome to our JSON Schema Repository for Payment Gateway Integration! This repository is dedicated to providing robust and comprehensive JSON schemas designed to streamline and standardize the integration of payment gateway systems in various applications. Our schemas are crafted to cater to a wide range of payment processing needs, including transaction handling, payment methods, customer details, and refund processes.

The purpose of these schemas is to offer developers a reliable and consistent structure for payment data, ensuring seamless interoperability between different systems and components in the e-commerce and online transaction space. Whether you're building a new e-commerce platform, integrating a payment gateway into an existing system, or developing tools for financial transactions, these schemas are designed to simplify your development process and enhance data integrity.

Our repository is community-driven and open to contributions. We encourage collaboration and feedback to continuously improve and update the schemas in line with the latest industry standards and practices. Let's work together to make online payment processing easier, safer, and more efficient for everyone.

## Cloud Events

For our ecosystem we are using Cloud Events in Binary Mode. The Cloud Events specification can be found [here](https://github.com/cloudevents/spec/blob/main/cloudevents/spec.md)

| Bounded Context     | Json Schema                                                                                                       | CloudEvent type                                           | Sample                                                                                                            |
|---------------------|-------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------|
| Payment Processing  | [paymentCreated](payment-processing/payments-gateway.v1.payment-created.json)                                     | paymentic.io.payment-processing.v1.payment.created        | [Payment Created](cloud-events-samples/payment-processing/payments-gateway.v1.payment-created.json)               |
| Payment Processing  | [refundCreated](payment-processing/payments-gateway.v1.refund-created.json)                                       | paymentic.io.payment-processing.v1.refund.created         | [Refund Created](cloud-events-samples/payment-processing/payments-gateway.v1.refund-created.json)                 |
| Payment Processing  | [paymentOrderDeclined](payment-processing/payments-gateway.v1.payment-order-declined.json)                        | paymentic.io.payment-processing.v1.payment-order.declined | ---------                                                                                                         |
| Payment Processing  | [paymentOrderStarted](payment-processing/payments-gateway.v1.payment-order-started.json)                          | paymentic.io.payment-processing.v1.payment-order.started  | [Payment Order Started](cloud-events-samples/payment-processing/payments-gateway.v1.payment-order-started.json)   |
| Payment Processing  | [paymentOrderApproved](payment-processing/payments-gateway.v1.payment-order-approved.json)                        | paymentic.io.payment-processing.v1.payment-order.approved | [Payment Order Approved](cloud-events-samples/payment-processing/payments-gateway.v1.payment-order-approved.json) |
| Merchant Account    | [transactionWalletRegistered](merchant-account-management/payments-gateway.v1.transaction-wallet-registered.json) | paymentic.io.merchant-account.v1.transaction.registered   | ---------                                                                                                         |
| Financial Recording | [transactionBooked](financial-recording-reporting/payments-gateway.v1.transaction-booked.json)                    | paymentic.io.financial-reporting.v1.transaction.booked    | ---------                                                                                                         |
