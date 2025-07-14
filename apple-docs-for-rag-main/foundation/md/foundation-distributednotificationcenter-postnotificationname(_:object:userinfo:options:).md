

- Foundation
- DistributedNotificationCenter
-  postNotificationName(\_:object:userInfo:options:) 

Instance Method

# postNotificationName(\_:object:userInfo:options:)

Creates a notification with information, and posts it to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func postNotificationName(
    _ name: NSNotification.Name,
    object: String?,
    userInfo: [AnyHashable : Any]? = nil,
    options: DistributedNotificationCenter.Options = []
)
```

## Parameters 

`name`  

Name of the notification to post. Must not be `nil`.

`object`  

Sender of the notification. May be `nil`.

`userInfo`  

Dictionary containing additional information. May be `nil`.

Important

Sandboxed apps can send notifications only if they do not contain a dictionary. If the sending application is in an App Sandbox, `userInfo` *must* be `nil`.

`options`  

Specifies how the notification is posted to the task and when to deliver it to its observers. See `Notification Posting Behavior` for details.

## Discussion

The `userInfo` dictionary is serialized as a property list, so it can be passed to another task. In the receiving task, it is deserialized back into a dictionary. This serialization imposes some restrictions on the objects that can be placed in the `userInfo` dictionary. See XML Property Lists for details.

## See Also

### Posting Notifications

func post(name: NSNotification.Name, object: String?)

Creates a notification, and posts it to the receiver.

func post(name: NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?)

Creates a notification with information, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, deliverImmediately: Bool)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

