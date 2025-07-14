

- StoreKit
- In-App Purchase
- Original API for In-App Purchase
-  Subscriptions and offers 

API Collection

# Subscriptions and offers

Offer customers additional time-based content and services through purchases they make within your app.

## Topics

### Essentials

Handling Subscriptions Billing

Build logic around the date and time constraints of subscription products, while planning for all scenarios where you control access to content.

Enabling App Store Server Notifications

Configure your server and provide an HTTPS URL to receive notifications about in-app purchase events and unreported external purchase tokens.

Offering a Subscription Across Multiple Apps

Support a single auto-renewable subscription across multiple apps.

Reducing Involuntary Subscriber Churn

Prevent unintentional loss of subscribers due to billing issues.

### Introductory offers

Provide discount pricing for new customers to encourage them to subscribe.

Implementing introductory offers in your app

Offer introductory pricing for auto-renewable subscriptions to eligible users.

Testing introductory offers

Test your introductory pricing in a variety of user scenarios.

class SKProductDiscount

The details of an introductory offer or a promotional offer for an auto-renewable subscription.

Deprecated

### Promotional offers

Provide discount pricing for existing or previously subscribed customers to encourage them to renew.

Setting up promotional offers

Generate a key and configure offers for auto-renewable subscriptions in App Store Connect.

Implementing promotional offers in your app

Offer discounted pricing for auto-renewable subscription products to eligible subscribers.

Generating a signature for promotional offers

Create a signature to validate a promotional offer using your private key.

Generating a Promotional Offer Signature on the Server

Generate a signature using your private key and lightweight cryptography libraries.

class SKPaymentDiscount

The signed discount to apply to a payment.

Deprecated

### Subscription offer codes

Provide offer codes to customers to acquire, retain, and win back subscribers.

Implementing offer codes in your app

Provide subscription service for customers who redeem offer codes through the App Store or within an app that uses receipts.

### Subscription service entitlement

Determining service entitlement on the server

Identify a customer’s entitlement to your service, offers, and messaging by analyzing a validated receipt and the state of their subscription.

