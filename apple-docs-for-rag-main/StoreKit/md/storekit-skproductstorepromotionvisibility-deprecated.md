

- StoreKit
-  SKProductStorePromotionVisibility Deprecated

Enumeration

# SKProductStorePromotionVisibility

The visibility settings that determine if an in-app purchase is visible on a device.

iOS 11.0–18.0DeprecatediPadOS 11.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 11.0–18.0Deprecated

``` source
@frozen
enum SKProductStorePromotionVisibility
```

Deprecated

Use Product.PromotionInfo.Visibility

## Topics

### Enumeration cases

case `default`

Indicates product visibility is the same as the default value set in App Store Connect.

case hide

Indicates product is hidden.

case show

Indicates product is shown.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing promoted product visibility

func fetchStorePromotionVisibility(for: SKProduct, completionHandler: ((SKProductStorePromotionVisibility, (any Error)?) -> Void)?)

Reads the visibility setting of a promoted product in the App Store for this device.

Deprecated

func update(storePromotionVisibility: SKProductStorePromotionVisibility, for: SKProduct, completionHandler: (((any Error)?) -> Void)?)

Updates the visibility of the product on the App Store, per device.

Deprecated

