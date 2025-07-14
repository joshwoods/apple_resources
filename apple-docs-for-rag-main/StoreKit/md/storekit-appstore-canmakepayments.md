

- StoreKit
- AppStore
-  canMakePayments 

Type Property

# canMakePayments

A Boolean value that indicates whether the person can make purchases.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var canMakePayments: Bool { get }
```

## Discussion

Use canMakePayments to determine at runtime whether a person can authorize payments. If the value is `false`, a person can’t authorize payments, so don’t offer In-App Purchases or external purchases.

Important

Your app might need to alter its behavior or appearance when people can’t make purchases. For example, don’t enable your user interface for making In-App Purchases or external purchases when purchases are blocked.

The following conditions can cause the value of canMakePayments to be `false`:

- A person sets the Content & Privacy Restrictions in Screen Time to prevent purchases. For more information, see Use parental controls on your child’s iPhone, iPad, and iPod touch.

- The device has a mobile device management (MDM) profile that prevents purchases. For more information, see Device Management.

If canMakePayments is `true` and your app uses only StoreKit In-App Purchase APIs, the person can authorize purchases in the App Store and your app can offer In-App Purchases.

### Determine whether to offer purchases for apps that use External Purchase APIs

If your app has the entitlements to use the External Purchase APIs, determine at runtime whether to use the External Purchase API or the In-App Purchase APIs by following these steps, in order:

1.  Check canMakePayments. If canMakePayments is `false`, don’t offer either external purchases or In-App Purchases. If canMakePayments if `true`, continue to step 2.

2.  Check the External Purchase API values: canOpen, canPresent, and isEligible. If any value is `true`, use only the External Purchase APIs to offer external purchases.

3.  If all the values (canOpen, canPresent, and isEligible) are `false`, and canMakePayments is `true`, use StoreKit In-App Purchase APIs to offer In-App Purchases.

Note

The StoreKit APIs always enable your app to view existing transactions and receive auto-renewable subscription renewals, so your app can support your customer’s existing purchases made through the App Store.

