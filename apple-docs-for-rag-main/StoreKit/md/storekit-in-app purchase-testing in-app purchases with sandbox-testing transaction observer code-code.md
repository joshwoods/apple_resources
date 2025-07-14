

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing transaction observer code 

Article

# Testing transaction observer code

Verify that your app activates its payment transaction observer by using breakpoints.

## Overview

Review the transaction observer’s implementation of the SKPaymentTransactionObserver protocol. Verify that the SKPaymentTransactionObserver listens for transactions when:

- Your app isn’t displaying its store UI

- If you didn’t recently initiate a purchase

Locate the call to the add(_:) method of SKPaymentQueue in your code. Verify that your app calls this method at app launch. For more information, see Setting up the transaction observer for the payment queue.

## See Also

### Transaction observer

Testing a successful transaction

Confirm that your app can make a successful transaction in the sandbox environment by inspecting the transaction.

Testing complete transactions

Verify that your app completes transactions properly by confirming that any downloadable purchases are present on your test device.

