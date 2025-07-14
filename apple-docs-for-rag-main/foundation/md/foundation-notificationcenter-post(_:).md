

- Foundation
- NotificationCenter
-  post(\_:) 

Instance Method

# post(\_:)

Posts a given notification to the notification center.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func post(_ notification: Notification)
```

## Parameters 

`notification`  

The notification to post.

## See Also

### Posting Notifications

func post(name: NSNotification.Name, object: Any?, userInfo: [AnyHashable : Any]?)

Creates a notification with a given name, sender, and information and posts it to the notification center.

func post(name: NSNotification.Name, object: Any?)

Creates a notification with a given name and sender and posts it to the notification center.

