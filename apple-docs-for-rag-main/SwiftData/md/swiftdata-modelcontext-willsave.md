

- SwiftData
- ModelContext
-  willSave 

Type Property

# willSave

A notification that posts when the context is about to process pending inserts, changes, and deletes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
static let willSave: Notification.Name
```

## Discussion

Note

Notifications with this name don’t contain a `userInfo` dictionary.

## See Also

### Registering for notifications

static let didSave: Notification.Name

A notification that posts when the context finishes processing pending inserts, changes, and deletes.

enum NotificationKey

Describes the data in the user info dictionary of a notification sent by a model context.

