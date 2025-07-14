

- StoreKit
- In-App Purchase
-  Original API for In-App Purchase 

API Collection

# Original API for In-App Purchase

Offer additional content and services in your app using the Original In-App Purchase API.

## Overview

The In-App Purchase APIs, including the original API and the Swift-based In-App Purchase API, allow you to offer customers the opportunity to purchase in-app content and features. Customers can make the purchases within your app, and find your promoted products on the App Store.

The StoreKit framework connects to the App Store on your app’s behalf to prompt for, and securely process, payments. The framework then notifies your app, which delivers the purchased products. To validate purchases, you can verify receipts on your server with the App Store or on the device. For auto-renewable subscriptions, the App Store can also notify your server of key subscription events.

For more information about In-App Purchases, including configuration, testing, marketing, and more, see In-App Purchase.

### Configure In-App Purchases in App Store Connect

To use the In-App Purchase API, you need to configure the products in App Store Connect. As you develop your app, you can add or remove products and refine or reconfigure existing products. For more information, see Configure In-App Purchase settings.

You can also offer apps and In-App Purchases that run on multiple platforms as a single purchase. For more information about universal purchase, see App Store Connect Help.

### Understand product types

There are four In-App Purchase types you can offer:

- *Consumables* are a type that are depleted after one use. Customers can purchase them multiple times.

- *Non-consumables* are a type that customers purchase once. They don’t expire. Non-consumable In-App Purchases can offer Family Sharing.

- *Auto-renewable subscriptions* to services or content are a type that customers purchase once and that renew automatically on a recurring basis until customers decide to cancel. Auto-renewable subscriptions can offer Family Sharing.

- *Non-renewing subscriptions* to services or content provide access over a limited duration and don’t renew automatically. Customers need to purchase a new subscription after it concludes if they want to retain access.

You can sync and restore non-consumables and auto-renewable subscriptions across devices using StoreKit. When a customer purchases an auto-renewable or non-renewing subscription, your app is responsible for making it available across all the person’s devices, and for restoring past purchases.

## Topics

### Essentials

Setting up the transaction observer for the payment queue

Enable your app to receive and handle transactions by adding an observer.

Offering, completing, and restoring in-app purchases

Fetch, display, purchase, validate, and finish transactions in your app.

class SKPaymentQueue

A queue of payment transactions for the App Store to process.

Deprecated

protocol SKPaymentTransactionObserver

A set of methods that process transactions, unlock purchased functionality, and continue promoted In-App Purchases.

Deprecated

protocol SKPaymentQueueDelegate

The protocol that provides information needed to complete transactions.

Deprecated

class SKRequest

An abstract class that represents a request to the App Store.

Deprecated

### Product information

Loading in-app product identifiers

Load the unique identifiers for your in-app products to retrieve product information from the App Store.

Fetching product information from the App Store

Retrieve up-to-date information about the products for sale in your app to display to your customers.

class SKProductsRequest

An object that can retrieve localized information from the App Store about a specified list of products.

Deprecated

class SKProductsResponse

An App Store response to a request for information about a list of products.

Deprecated

class SKProduct

Information about a registered product in App Store Connect.

Deprecated

### Storefronts

class SKStorefront

An object containing the location and unique identifier of an Apple App Store storefront.

Deprecated

### Purchases

Requesting a payment from the App Store

Submit a payment request to the App Store when a customer selects a product to buy.

Processing a transaction

Register a transaction queue observer to get and handle transaction updates from the App Store.

class SKPayment

A request to the App Store to process payment for additional functionality that your app offers.

Deprecated

class SKMutablePayment

A mutable request to the App Store to process payment for additional functionality that your app offers.

Deprecated

class SKPaymentTransaction

An object in the payment queue.

Deprecated

### Purchase validation

Choosing a receipt validation technique

Select the type of receipt validation, on the device or on your server, that works for your app.

Validating receipts with the App Store

Verify transactions with the App Store on a secure server.

var appStoreReceiptURL: URL?

The file URL for the bundle’s App Store receipt.

class SKReceiptRefreshRequest

A request to the App Store to get the app receipt, which represents the customer’s transactions with your app.

Deprecated

### Content delivery

Unlocking purchased content

Deliver content to the customer after validating the purchase.

Persisting a purchase

Keep a persistent record of a purchase to continue making the product available as needed.

Finishing a transaction

Finish the transaction to complete the purchase process.

class SKDownload

Downloadable content associated with a product.

Deprecated

### Refunds

Handling refund notifications

Respond to notifications about customer refunds for consumable, non-consumable, and non-renewing subscription products.

Testing refund requests

Test your app’s implementation of refund requests, and your app’s and server’s handling of approved and declined refunds.

### Providing access to previously purchased products

Restoring purchased products

Give customers functionality that restores their purchases in your app to maintain access to purchased content.

class SKReceiptRefreshRequest

A request to the App Store to get the app receipt, which represents the customer’s transactions with your app.

Deprecated

class SKRequest

An abstract class that represents a request to the App Store.

Deprecated

class SKPaymentTransaction

An object in the payment queue.

Deprecated

func SKTerminateForInvalidReceipt()

Terminates an app if the license to use the app has expired.

### Family Sharing

Supporting Family Sharing in your app

Provide service to share subscriptions and non-consumable products to family members.

var isFamilyShareable: Bool

A Boolean value that indicates whether the product is available for Family Sharing in App Store Connect.

Deprecated

func paymentQueue(SKPaymentQueue, didRevokeEntitlementsForProductIdentifiers: [String])

Tells an observer that the customer is no longer entitled to one or more Family Sharing purchases.

Deprecated

### Subscriptions

Subscriptions and offers

Offer customers additional time-based content and services through purchases they make within your app.

### Promotions

Promoting In-App Purchases

Show promoted In-App Purchases on your product page and handle purchases that customers initiate on the App Store.

Testing promoted In-App Purchases

Test your In-App Purchases before making your app available in the App Store.

class SKProductStorePromotionController

A product promotion controller for customizing the order and visibility of In-App Purchases per device.

Deprecated

### Testing In-App Purchases

Testing at all stages of development with Xcode and the sandbox

Verify your implementation of In-App Purchases by testing your code throughout its development.

Setting up StoreKit Testing in Xcode

Prepare your test environment to test in-app purchases with data you configure locally.

Testing In-App Purchases in Xcode

Use locally configured product data to test and debug your In-App Purchases implementation.

Testing In-App Purchases with sandbox

Test your implementation of In-App Purchases using real product information and server-to-server transactions in the sandbox environment.

### Errors

Handling errors

Determine the underlying cause of errors that result from StoreKit requests.

enum Code

Error codes for StoreKit errors.

struct SKError

StoreKit error descriptions, codes, and domains.

let SKErrorDomain: String

The error domain name for StoreKit errors.

## See Also

### Deprecated

Choosing a StoreKit API for In-App Purchases

Use the latest API to support In-App Purchases in new or existing apps, or the original API to support In-App Purchases in earlier operating systems.

