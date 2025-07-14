

- StoreKit
-  SKStoreReviewController Deprecated

Class

# SKStoreReviewController

An object that controls the process of requesting App Store ratings and reviews from customers.

iOS 10.3–18.0DeprecatediPadOS 10.3–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.14–15.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
class SKStoreReviewController
```

Deprecated

Use RequestReviewAction instead.

## Overview

Use the requestReview(in:) method to indicate when it makes sense within the logic of your app to ask the customer for ratings and reviews.

## Topics

### Indicating an appropriate time for a review

class func requestReview(in: UIWindowScene)

Tells StoreKit to ask the customer to rate or review the app, if appropriate, using the specified scene.

class func requestReview()

Tells StoreKit to ask the customer to rate or review your app, if appropriate.

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
- Sendable

## See Also

### Reviews

Requesting App Store reviews

Implement best practices for prompting users to review your app in the App Store.

struct RequestReviewAction

An instance that tells StoreKit to request an App Store rating or review, if appropriate.

