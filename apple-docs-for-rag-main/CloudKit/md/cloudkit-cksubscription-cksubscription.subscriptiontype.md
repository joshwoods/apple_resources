

- CloudKit
- CKSubscription
-  CKSubscription.SubscriptionType 

Enumeration

# CKSubscription.SubscriptionType

Constants that identify a subscription’s behavior.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 6.0+

``` source
enum SubscriptionType
```

## Topics

### Subscription Types

case query

A constant that indicates the subscription is query-based.

case database

A constant that indicates the subscription is database-based.

case recordZone

A constant that indicates the subscription is zone-based.

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

### Accessing the Subscription Metadata

var subscriptionID: CKSubscription.ID

The subscription’s unique identifier.

typealias ID

A type that represents a subscription’s identifier.

var subscriptionType: CKSubscription.SubscriptionType

The behavior that a subscription provides.

