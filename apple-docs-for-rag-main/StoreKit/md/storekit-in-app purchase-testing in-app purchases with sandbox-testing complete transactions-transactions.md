

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing complete transactions 

Article

# Testing complete transactions

Verify that your app completes transactions properly by confirming that any downloadable purchases are present on your test device.

## Overview

Locate where your app calls the finishTransaction(_:) method, and verify that your app completes all work related to the transaction before calling the method. For example, if the purchase includes downloadable content, verify your app downloaded the content to your test device as described in Persisting a purchase. Verify that you call finishTransaction(_:) for every transaction, whether it succeeded or failed. For more information, see Finishing a transaction.

## See Also

### Transaction observer

Testing transaction observer code

Verify that your app activates its payment transaction observer by using breakpoints.

Testing a successful transaction

Confirm that your app can make a successful transaction in the sandbox environment by inspecting the transaction.

