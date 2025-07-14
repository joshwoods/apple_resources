

- Foundation
- NotificationCenter
-  NotificationCenter.Publisher 

Structure

# NotificationCenter.Publisher

A publisher that emits elements when broadcasting notifications.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Publisher
```

## Topics

### Creating a Notification Publisher

init(center: NotificationCenter, name: Notification.Name, object: AnyObject?)

Creates a publisher that emits events when broadcasting notifications.

### Inspecting Notification Center Properties

let center: NotificationCenter

The notification center this publisher uses as a source.

let name: Notification.Name

The name of notifications published by this publisher.

let object: AnyObject?

The object posting the named notfication.

## Relationships

### Conforms To

- Copyable
- Equatable
- Publisher

## See Also

### Receiving Notifications as a Combine Publisher

func publisher(for: Notification.Name, object: AnyObject?) -> NotificationCenter.Publisher

Returns a publisher that emits events when broadcasting notifications.

