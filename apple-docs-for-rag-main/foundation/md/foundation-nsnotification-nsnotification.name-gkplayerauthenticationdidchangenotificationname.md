

- Foundation
- NSNotification
- NSNotification.Name
-  GKPlayerAuthenticationDidChangeNotificationName 

Type Property

# GKPlayerAuthenticationDidChangeNotificationName

A notification that posts after GameKit authenticates the local player.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
static let GKPlayerAuthenticationDidChangeNotificationName: NSNotification.Name
```

## Discussion

The object property for this notification is a `GKLocalPlayer` object. Passing `nil` provides standard Notification Center behavior, which is to receive the notification for any object.

## See Also

### GameKit

static let GKPlayerDidChangeNotificationName: NSNotification.Name

A notification that posts when a player object’s data changes.

