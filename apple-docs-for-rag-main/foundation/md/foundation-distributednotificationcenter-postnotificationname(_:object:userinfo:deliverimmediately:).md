

- Foundation
- DistributedNotificationCenter
-  postNotificationName(\_:object:userInfo:deliverImmediately:) 

Instance Method

# postNotificationName(\_:object:userInfo:deliverImmediately:)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func postNotificationName(
    _ name: NSNotification.Name,
    object: String?,
    userInfo: [AnyHashable : Any]? = nil,
    deliverImmediately: Bool
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

`deliverImmediately`  

Specifies when to deliver the notification. When false, the receiver delivers notifications to their observers according to the suspended-notification behavior specified in the corresponding dispatch table entry. When true, the receiver delivers the notification immediately to its observers.

## Discussion

This is the preferred method for posting notifications.

The `notificationInfo` dictionary is serialized as a property list, so it can be passed to another task. In the receiving task, it is deserialized back into a dictionary. This serialization imposes some restrictions on the objects that can be placed in the `notificationInfo` dictionary. See XML Property Lists for details.

## See Also

### Related Documentation

class func unarchiveObject(with: Data) -> Any?

Decodes and returns the object archived in a given `NSData` object.

Deprecated

func encodeRootObject(Any)

Archives a given object along with all the objects to which it is connected.

Deprecated

### Posting Notifications

func post(name: NSNotification.Name, object: String?)

Creates a notification, and posts it to the receiver.

func post(name: NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?)

Creates a notification with information, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, options: DistributedNotificationCenter.Options)

Creates a notification with information, and posts it to the receiver.

