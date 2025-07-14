

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing an interrupted purchase 

Article

# Testing an interrupted purchase

Verify that your app handles an interrupted purchase by inspecting and invoking payment transactions.

## Overview

An interrupted purchase is a transaction that requires the user to perform some action outside of your app before completing their transaction. For example, the user may need to update their payment method or accept new terms and conditions before continuing with their transaction.

In sandbox testing, you can simulate an interrupted purchase by turning on the interrupted purchase feature in App Store Connect for a tester Sandbox Apple ID. This interrupts all purchase attempts by that Sandbox Apple ID until you agree to the updated terms and conditions on the iOS device, or until you turn off the feature in App Store Connect. To learn how to set up interrupted purchase testing, see Enable interrupted purchases for a Sandbox Apple ID.

### Set up testing

To enable interrupted purchases for the Sandbox Apple ID, log in to App Store Connect, and do the following:

1.  From Users and Access, open the Users and Access Panel in the sidebar, under the Sandbox header, select Testers. On the right, you can view your Sandbox Apple IDs.

2.  Select a Sandbox Apple ID to use for testing interrupted purchases. If it’s already enabled, you’ll see a checkmark under the Interrupted Purchases column.

3.  In the dialog that appears, select Interrupt Purchases for This Tester.

### Begin testing

After setting up interrupted purchase testing in App Store Connect, use the following steps to test your app:

1.  On the test device, sign in with the Sandbox Apple ID that has interrupted purchases enabled.

2.  In your app, select Buy or Subscribe to make an in-app purchase.

3.  Observe that the system displays a payment sheet.

4.  In Xcode, verify that the payment queue receives a new transaction in the state SKPaymentTransactionState.purchasing.

5.  On the device, authenticate the payment sheet.

6.  In Xcode, observe that the payment fails. The payment queue receives an updated transaction in the state SKPaymentTransactionState.failed.

7.  Check that your code calls finishTransaction(_:) to remove it from the queue.

8.  On the device, observe that the system displays Terms & Conditions, interrupting the purchase (because you configured the sandbox environment to do so).

9.  On the device, tap to agree to the Terms & Conditions.

10. In Xcode, verify that the payment queue receives a new transaction in the SKPaymentTransactionState.purchased state for the same productIdentifier and in the same quantity as the failed transaction.

11. In Xcode, validate the receipt. Check that your app provides the service or the product, and calls finishTransaction(_:).

12. On the device, the user should observe a successful purchase.

### Conclude testing

The Sandbox Apple ID continues to experience interrupted purchases until you disable it in App Store Connect, or until the user agrees to the terms and conditions on the device. To disable interrupted purchases in App Store Connect, deselect Interrupt Purchases for This Tester. For more information, see Enable interrupted purchases for a Sandbox Apple ID.

## See Also

### Payment transactions

Testing purchases made outside your app

Verify that your app receives and handles transactions that occur outside your app, such as subscription purchases, renewals, and offer and promo code redemptions.

Testing win-back offers in the sandbox environment

Verify that your app receives and handles win-back offer transactions, including those made outside your app.

Testing failing subscription renewals and In-App Purchases

Verify that your app handles failed subscription renewals that are in the billing retry or billing grace period states, as well as failed In-App Purchases.

Testing a payment request

Verify that requests for payment function properly in the sandbox environment by inspecting the calls to the payment transaction observer.

