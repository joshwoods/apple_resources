

- StoreKit
- In-App Purchase
- Original API for In-App Purchase
-  Requesting a payment from the App Store 

Article

# Requesting a payment from the App Store

Submit a payment request to the App Store when a customer selects a product to buy.

## Overview

After you present your app’s store UI, users can make purchases from within your app. When the user chooses a product, your app creates and submits a payment request to the App Store.

Implementing an in-app purchase flow consists of three stages. In the first stage, your app retrieves product information. Then your app requests payment when the user selects a product in your app’s store. Finally, your app delivers the products.

### Create a payment request

When the user selects a product to buy, create a payment request using the corresponding SKProduct object and set the quantity if needed, as the code below shows. The product object comes from the array of products that your app’s products request returns, as described in Fetching product information from the App Store.

- Swift
- Objective-C

```
// Use the corresponding SKProduct object that returns in the array from SKProductsRequest.
let payment = SKMutablePayment(product: product)
payment.quantity = 2
```

```
SKProduct *product = ;
SKMutablePayment *payment = [SKMutablePayment paymentWithProduct:product];
payment.quantity = 2;
```

### Submit a payment request

Submit your payment request to the App Store by adding it to the payment queue. If you add a payment object to the queue more than once, the system submits it to the App Store multiple times, charging the user and requiring your app to deliver the product each time.

- Swift
- Objective-C

```
SKPaymentQueue.default().add(payment)
```

```
[[SKPaymentQueue defaultQueue] addPayment:payment];
```

For each payment request your app submits, it receives a corresponding transaction to process. For more information about transactions and the payment queue, see Processing a transaction.

For auto-renewable subscriptions, you may submit a payment request with a subscription offer for users you determine eligible to receive an offer. For more information, see Implementing promotional offers in your app.

## See Also

### Purchases

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

