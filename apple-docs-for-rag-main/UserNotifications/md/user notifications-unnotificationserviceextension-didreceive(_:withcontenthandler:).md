

- User Notifications
- UNNotificationServiceExtension
-  didReceive(\_:withContentHandler:) 

Instance Method

# didReceive(\_:withContentHandler:)

Asks you to make any needed changes to the notification and notify the system when you’re done.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 6.0+

``` source
func didReceive(
    _ request: UNNotificationRequest,
    withContentHandler contentHandler: @escaping (UNNotificationContent) -> Void
)
```

## Parameters 

`request`  

The original notification request. Use this object to get the original content of the notification.

`contentHandler`  

The block to execute with the modified content. This block has no return value and takes the following parameter:

contentToDeliver  
A UNNotificationContent object with the content the system displays to the user.

## Mentioned in 

Modifying content in newly delivered notifications

Implementing communication notifications

## Discussion

Override this method and use it to modify the UNNotificationContent object that the system delivers with the notification. At some point during your implementation, execute the `contentHandler` block and pass it your modified content. If you decide not to modify the content, call the `contentHandler` block with the original content from the `request` parameter.

You can modify any of the content from the original request. You might customize the content for the current user or replace it altogether. You can use this method to download images or movies and add them as attachments to the content. You may also modify the alert text as long as you don’t remove it. If the content object doesn’t contain any alert text, the system ignores your modifications and delivers the original notification content.

Your extension has a limited amount of time (no more than 30 seconds) to modify the content and execute the `contentHandler` block. If you don’t execute that block in a timely manner, the system calls your extension’s serviceExtensionTimeWillExpire() method to give you one last chance to execute the block. If you don’t, the system presents the notification’s original content to the user.

## See Also

### Processing Notifications

func serviceExtensionTimeWillExpire()

Tells you that the system is terminating your extension.

