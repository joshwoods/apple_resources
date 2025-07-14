

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing a payment request 

Article

# Testing a payment request

Verify that requests for payment function properly in the sandbox environment by inspecting the calls to the payment transaction observer.

## Overview

Create an instance of SKPayment using a valid product identifier that you’ve already tested, as described in Testing fetching product identifiers. Set a breakpoint and inspect the payment request. Add the payment request to the transaction queue, and set a breakpoint to confirm that the system calls your observer’s paymentQueue(_:updatedTransactions:) method.

Though you can finish the transaction immediately without providing the content of the purchase during testing, failing to finish the transaction can cause problems. Unfinished transactions remain in the queue indefinitely, which could interfere with later testing. Complete the transaction as described in Finishing a transaction at the end of each test.

## See Also

### Payment transactions

Testing purchases made outside your app

Verify that your app receives and handles transactions that occur outside your app, such as subscription purchases, renewals, and offer and promo code redemptions.

Testing win-back offers in the sandbox environment

Verify that your app receives and handles win-back offer transactions, including those made outside your app.

Testing an interrupted purchase

Verify that your app handles an interrupted purchase by inspecting and invoking payment transactions.

Testing failing subscription renewals and In-App Purchases

Verify that your app handles failed subscription renewals that are in the billing retry or billing grace period states, as well as failed In-App Purchases.

