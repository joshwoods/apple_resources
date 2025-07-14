

- User Notifications
-  UNNotificationAttachmentOptionsThumbnailHiddenKey 

Global Variable

# UNNotificationAttachmentOptionsThumbnailHiddenKey

A Boolean value indicating whether the system hides the attachment’s thumbnail.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
let UNNotificationAttachmentOptionsThumbnailHiddenKey: String
```

## Discussion

The value of this key is an NSNumber containing a Boolean value. When set to true, the attachment’s thumbnail isn’t displayed. If you don’t include this key, the system shows the thumbnail.

## See Also

### Creating an Attachment

convenience init(identifier: String, url: URL, options: [AnyHashable : Any]?) throws

Creates an attachment object from the specified file and options.

let UNNotificationAttachmentOptionsTypeHintKey: String

A hint about an attachment’s file type.

let UNNotificationAttachmentOptionsThumbnailClippingRectKey: String

The clipping rectangle for a thumbnail image.

let UNNotificationAttachmentOptionsThumbnailTimeKey: String

The frame number of an animation to use as a thumbnail image.

