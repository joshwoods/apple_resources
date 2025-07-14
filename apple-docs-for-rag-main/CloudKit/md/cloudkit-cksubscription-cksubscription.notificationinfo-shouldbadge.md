

- CloudKit
- CKSubscription
- CKSubscription.NotificationInfo
-  shouldBadge 

Instance Property

# shouldBadge

A Boolean value that determines whether an app’s icon badge increments its value.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+watchOS 6.0+

``` source
var shouldBadge: Bool { get set }
```

## Discussion

The default value of this property is false. Set it to true to cause the system to increment the badge value whenever it receives the corresponding push notification.

