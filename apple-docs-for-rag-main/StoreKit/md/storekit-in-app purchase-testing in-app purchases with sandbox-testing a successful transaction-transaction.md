

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing a successful transaction 

Article

# Testing a successful transaction

Confirm that your app can make a successful transaction in the sandbox environment by inspecting the transaction.

## Overview

Set a breakpoint in your implementation of the transaction queue observer’s paymentQueue(_:updatedTransactions:) method. Then sign in to the App Store with a Sandbox Apple ID, and make a purchase in your app. Inspect the transaction to verify that its status is SKPaymentTransactionState.purchased.

Set a breakpoint at the point in your code where your app stores the purchase, and confirm that your code saves the data in response to a successful purchase. Inspect the user default or iCloud key-value store, to verify that your code correctly records the information. For more information on saving data in response to a successful purchase, see Persisting a purchase.

## See Also

### Transaction observer

Testing transaction observer code

Verify that your app activates its payment transaction observer by using breakpoints.

Testing complete transactions

Verify that your app completes transactions properly by confirming that any downloadable purchases are present on your test device.

