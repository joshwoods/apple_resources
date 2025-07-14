

- SwiftData
- ModelContext
-  didSave 

Type Property

# didSave

A notification that posts when the context finishes processing pending inserts, changes, and deletes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
static let didSave: Notification.Name
```

## Discussion

The notification’s `userInfo` dictionary contains the persistent identifiers of any inserted, updated, or deleted models. Use the appropriate key to access those identifiers. For more information, see ModelContext.NotificationKey.

## See Also

### Registering for notifications

static let willSave: Notification.Name

A notification that posts when the context is about to process pending inserts, changes, and deletes.

enum NotificationKey

Describes the data in the user info dictionary of a notification sent by a model context.

