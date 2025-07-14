

- Foundation
- DistributedNotificationCenter
-  post(name:object:) 

Instance Method

# post(name:object:)

Creates a notification, and posts it to the receiver.

Mac Catalyst 13.0+macOS 10.0+

``` source
func post(
    name aName: NSNotification.Name,
    object anObject: String?
)
```

## Parameters 

`aName`  

Name of the notification to post. Must not be `nil`.

`anObject`  

Sender of the notification. May be `nil`.

## Discussion

This method invokes postNotificationName(_:object:userInfo:deliverImmediately:) with `userInfo:nil deliverImmediately:NO`.

## See Also

### Posting Notifications

func post(name: NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?)

Creates a notification with information, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, deliverImmediately: Bool)

Creates a notification with information and an immediate-delivery specifier, and posts it to the receiver.

func postNotificationName(NSNotification.Name, object: String?, userInfo: [AnyHashable : Any]?, options: DistributedNotificationCenter.Options)

Creates a notification with information, and posts it to the receiver.

