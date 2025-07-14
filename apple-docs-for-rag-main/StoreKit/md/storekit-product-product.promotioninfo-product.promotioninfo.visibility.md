

- StoreKit
- Product
- Product.PromotionInfo
-  Product.PromotionInfo.Visibility 

Enumeration

# Product.PromotionInfo.Visibility

The visibility states for product promotion information.

iOS 16.4+iPadOS 16.4+

``` source
enum Visibility
```

## Overview

Use the visibility states to set the visibility of a promoted in-app purchase. Call update() to save your changes.

The visibility states have the following effects on the user’s device:

- Product.PromotionInfo.Visibility.visible makes the promoted in-app purchase visible in the App Store.

- Product.PromotionInfo.Visibility.hidden hides the promoted in-app purchase in the App Store.

- Product.PromotionInfo.Visibility.appStoreConnectDefault let’s you control the visibility using settings in App Store Connect. For more information, see Promote in-app purchases.

## Topics

### Getting visibility states

case appStoreConnectDefault

A visibility value for a promoted in-app purchase that uses the visibility setting from App Store Connect.

case hidden

A visibility value that hides a promoted in-app purchase on the App Store on a user’s device.

case visible

A visibility value that makes a promoted in-app purchase visible on the App Store on a user’s device.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable

## See Also

### Managing promotion visibility

var visibility: Product.PromotionInfo.Visibility

A value that indicates whether the promoted in-app purchase is visible or hidden on the user’s device.

static func updateProductVisibility(Product.PromotionInfo.Visibility, for: Product.ID) async throws

Updates a value that indicates whether a promoted in-app purchase appears in the App Store on the user’s device.

