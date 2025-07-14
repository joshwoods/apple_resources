

- User Notifications
- UNNotificationServiceExtension
-  serviceExtensionTimeWillExpire() 

Instance Method

# serviceExtensionTimeWillExpire()

Tells you that the system is terminating your extension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 6.0+

``` source
func serviceExtensionTimeWillExpire()
```

## Mentioned in 

Modifying content in newly delivered notifications

## Discussion

If your didReceive(_:withContentHandler:) method takes too long to execute its completion block, the system calls this method on a separate thread to give you one last chance to execute the block. Use this method to execute the block as quickly as possible. Doing so might mean providing some fallback content. For example, if your extension is still downloading an image file with the intent of attaching it to the notification’s content, update the notification’s alert text to indicate that an image download is in progress. If you fail to execute the completion block from the didReceive(_:withContentHandler:) method in time, the system displays the notification’s original content.

## See Also

### Processing Notifications

func didReceive(UNNotificationRequest, withContentHandler: (UNNotificationContent) -> Void)

Asks you to make any needed changes to the notification and notify the system when you’re done.

