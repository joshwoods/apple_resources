

- Foundation
- NotificationCenter
-  publisher(for:object:) 

Instance Method

# publisher(for:object:)

Returns a publisher that emits events when broadcasting notifications.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func publisher(
    for name: Notification.Name,
    object: AnyObject? = nil
) -> NotificationCenter.Publisher
```

## Parameters 

`name`  

The name of the notification to publish.

`object`  

The object posting the named notification. If `nil`, the publisher emits elements for any object producing a notification with the given name.

## Return Value

A Publisher that emits events when broadcasting notifications.

## See Also

### Receiving Notifications as a Combine Publisher

struct Publisher

A publisher that emits elements when broadcasting notifications.

