

- User Notifications
-  UNNotificationAttachmentOptionsTypeHintKey 

Global Variable

# UNNotificationAttachmentOptionsTypeHintKey

A hint about an attachment’s file type.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
let UNNotificationAttachmentOptionsTypeHintKey: String
```

## Discussion

The value of this key is an NSString containing a Uniform Type Identifier (UTI) that describes the file’s type. If you don’t include this key, the system uses the attachment’s filename extension to determine its type.

## See Also

### Creating an Attachment

convenience init(identifier: String, url: URL, options: [AnyHashable : Any]?) throws

Creates an attachment object from the specified file and options.

let UNNotificationAttachmentOptionsThumbnailHiddenKey: String

A Boolean value indicating whether the system hides the attachment’s thumbnail.

let UNNotificationAttachmentOptionsThumbnailClippingRectKey: String

The clipping rectangle for a thumbnail image.

let UNNotificationAttachmentOptionsThumbnailTimeKey: String

The frame number of an animation to use as a thumbnail image.

