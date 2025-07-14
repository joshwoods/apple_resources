

- Foundation
- DistributedNotificationCenter
-  post(name:object:userInfo:) 

Instance Method

# post(name:object:userInfo:)

Creates a notification with information, and posts it to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func post(
    name aName: NSNotification.Name,
    object anObject: String?,
    userInfo aUserInfo: [AnyHashable : Any]? = nil
)
```

## Parameters 

`aName`  

Name of the notification to post. Must not be `nil`.

`anObject`  

Sender of the notification. May be `nil`.

`aUserInfo`  

Dictionary containing additional information. May be `nil`.

Important

Sandboxed apps can send notifications only if they do not contain a dictionary. If the sending application is in an App Sandbox, `notificationInfo` *must* be `nil`.

## Discussion

This method invokes postNotificationName(_:object:userInfo:deliverImmediately:) with `deliverImmediately:NO`.

## See Also

### Posting Notifications

func post(name: NSNotification.Name, object: String?)

Creates a notification, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, deliverImmediately: Bool)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, options: DistributedNotificationCenter.Options)

Creates a notification with information, and posts it to the receiver.

