

- StoreKit
-  SKProductStorePromotionController Deprecated

Class

# SKProductStorePromotionController

A product promotion controller for customizing the order and visibility of In-App Purchases per device.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
class SKProductStorePromotionController
```

Deprecated

Use Product.PromotionInfo

## Mentioned in 

Promoting In-App Purchases

## Overview

For information about promoting In-App Purchases, see Promoting In-App Purchases.

Note

SKProductStorePromotionController and promoted In-App Purchases aren’t available to compatible iPad and iPhone apps running in visionOS.

## Topics

### Managing promoted product order

func fetchStorePromotionOrder(completionHandler: (([SKProduct], (any Error)?) -> Void)?)

Reads the product order override that determines the promoted product order on this device.

func update(storePromotionOrder: [SKProduct], completionHandler: (((any Error)?) -> Void)?)

Overrides the promoted product order on this device.

### Managing promoted product visibility

func fetchStorePromotionVisibility(for: SKProduct, completionHandler: ((SKProductStorePromotionVisibility, (any Error)?) -> Void)?)

Reads the visibility setting of a promoted product in the App Store for this device.

func update(storePromotionVisibility: SKProductStorePromotionVisibility, for: SKProduct, completionHandler: (((any Error)?) -> Void)?)

Updates the visibility of the product on the App Store, per device.

enum SKProductStorePromotionVisibility

The visibility settings that determine if an in-app purchase is visible on a device.

### Getting the controller

class func `default`() -> Self

Returns the default product store promotion controller.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Promotions

Promoting In-App Purchases

Show promoted In-App Purchases on your product page and handle purchases that customers initiate on the App Store.

Testing promoted In-App Purchases

Test your In-App Purchases before making your app available in the App Store.

