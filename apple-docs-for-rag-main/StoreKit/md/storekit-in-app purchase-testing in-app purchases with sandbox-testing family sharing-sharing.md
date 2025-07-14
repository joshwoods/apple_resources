

- StoreKit
- In-App Purchase
- Testing In-App Purchases with sandbox
-  Testing Family Sharing 

Article

# Testing Family Sharing

Verify that your app handles auto-renewable subscriptions and non-consumable in-app purchases that family members share with Family Sharing.

## Overview

Family Sharing lets people share access to auto-renewable subscriptions or non-consumables that have Family Sharing enabled with up to five family members. You can use Sandbox Test Families to test whether your app works with Family Sharing as expected.

Note

Changes that you make to product metadata in App Store Connect can take up to one hour to appear in the sandbox environment.

To test Family Sharing in your app:

- Ensure your in-app purchases are set up to support Family Sharing. For more information, see Turn on Family Sharing for in-app purchases.

- Create two or more Sandbox Apple Accounts to add to a Sandbox Test Family, or use existing accounts. A family group can have up to six members. For more information, see Create a Sandbox Apple Account.

- Create the Sandbox Test Family in App Store Connect. For more information, see Create a Sandbox Test Family.

- To make testing easier, have a separate device to use for each test family member. You can also use a single device and sign in using each family member’s Sandbox Apple Account in turn.

### Manage sharing for the Sandbox Test Family

You can set the sharing status for each member of the Sandbox Test Family individually, as follows:

- *Sharing* indicates the family member shares their in-app purchases with the Sandbox Test Family, and gets access to in-app purchases shared by family members.

- *Not Sharing* indicates the family member isn’t sharing, and doesn’t get access to family-shared purchases. Changing the setting to Not Sharing revokes any family-shared purchases they have access to. In the test environment, turning off sharing is the equivalent of a family member leaving the group.

Modify the sharing status on the Family Sharing page in iOS by following these steps:

1.  Open Settings and select Developer.

2.  Select the Sandbox Apple Account.

3.  On the popup sheet, select Manage.

4.  On the Account Settings page, select Family Sharing.

5.  Select a family member.

6.  Select Stop Sharing Purchases or Start Sharing Purchases, as appropriate.

You can also change these settings in App Store Connect. For more information, see Manage a Sandbox Test Family.

### Test sharing an in-app purchase in a family group

The two main test cases for Family Sharing are a family member gaining and losing access to family-shared purchases. You can simulate these situations as follows.

To test family members gaining access to a shared purchase:

1.  Start with a Sandbox Test Family where members are sharing.

2.  In your app, purchase a shareable product.

3.  Open your app on a device signed in with the Sandbox Apple Account of another test family member.

4.  Verify that your app receives a transaction for the shared purchase and unlocks the content for the family member. Note that the transaction has a familyShared ownership type.

5.  When sharing auto-renewable subscriptions, if you have App Store Server Notifications V2 enabled in the sandbox environment, your server receives a notification for each test family member that has sharing enabled. For more information, see the `SUBSCRIBED` notificationType.

### Test revoked access to shared in-app purchases

To test a family member losing access to shared purchases:

1.  Start with a Sandbox Test Family with two or more members, and at least one shared purchase.

2.  In Account Settings \> Family Sharing, select a test family member that is receiving access to a shared in-app purchase.

3.  Select Stop Sharing Purchases, and Stop Sharing to confirm.

4.  The test family member loses accesses to shared purchases. Open your app using their Sandbox Apple Account and confirm that your app receives an updated transaction that includes a revocationDate and revocationReason.

5.  If you have App Store Server Notifications V2 enabled in the sandbox environment, your server receives a `REVOKE` notificationType for the test family member that has sharing disabled.

Note that you can also change the sharing status using App Store Connect instead of Account Settings in iOS.

