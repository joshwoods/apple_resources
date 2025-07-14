

- StoreKit
- SKPaymentQueue
-  restoreCompletedTransactions() Deprecated

Instance Method

# restoreCompletedTransactions()

Asks the payment queue to restore previously completed purchases.

iOS 3.0–18.0DeprecatediPadOS 3.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.7–15.0DeprecatedtvOS 9.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 6.2–11.0Deprecated

``` source
func restoreCompletedTransactions()
```

Deprecated

Use AppStore.sync()

## Mentioned in 

Choosing a receipt validation technique

Validating receipts with the App Store

Testing In-App Purchases in Xcode

Restoring purchased products

## Discussion

Use this method to restore finished transactions—that is, transactions for which you have already called finishTransaction(_:). You call this method in one of the following situations:

- To install purchases on additional devices

- To restore purchases for an application that the user deleted and reinstalled

When you create a new product to be sold in your store, you choose whether that product can be restored or not. See the In-App Purchase Programming Guide for more information.

The payment queue delivers a new transaction for each previously completed transaction that can be restored. Each transaction includes a copy of the original transaction.

After the transactions are delivered, the payment queue calls the observer’s paymentQueueRestoreCompletedTransactionsFinished(_:) method. If an error occurred while restoring transactions, the observer will be notified through its paymentQueue(_:restoreCompletedTransactionsFailedWithError:) method.

This method has no effect in the following situations:

- All transactions are unfinished.

- The user did not purchase anything that is restorable.

- You tried to restore items that are not restorable, such as a non-renewing subscription or a consumable product.

- Your app’s build version does not meet the guidelines for the `CFBundleVersion` key.

Important

If you are using the In-App Purchase API and managing transactions using the Transaction API, use currentEntitlements to determine which in-app purchases the customer is currently entitled to. The restoreCompletedTransactions() function doesn’t affect transactions in the Transaction API. In rare cases when a user suspects the app isn’t showing all the transactions, call sync() in response to an explicit user action, like tapping a button.

## See Also

### Restoring Purchases

func restoreCompletedTransactions(withApplicationUsername: String?)

Asks the payment queue to restore previously completed purchases, providing an opaque identifier for the user’s account.

Deprecated

