

- User Notifications
-  UNNotificationAttachmentOptionsThumbnailClippingRectKey 

Global Variable

# UNNotificationAttachmentOptionsThumbnailClippingRectKey

The clipping rectangle for a thumbnail image.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
let UNNotificationAttachmentOptionsThumbnailClippingRectKey: String
```

## Discussion

The value of this key is a dictionary containing a normalized CGRect — a unit rectangle whose values are in the range `0.0` to `1.0` and represent the portion of the original image that you want to display. For example, specifying an origin of (`0.25`, `0.25`) and a size of (`0.5`, `0.5`) defines a clipping rectangle that shows only the center portion of the image. Use the dictionaryRepresentation function to create the dictionary for your rectangle.

## See Also

### Creating an Attachment

convenience init(identifier: String, url: URL, options: [AnyHashable : Any]?) throws

Creates an attachment object from the specified file and options.

let UNNotificationAttachmentOptionsTypeHintKey: String

A hint about an attachment’s file type.

let UNNotificationAttachmentOptionsThumbnailHiddenKey: String

A Boolean value indicating whether the system hides the attachment’s thumbnail.

let UNNotificationAttachmentOptionsThumbnailTimeKey: String

The frame number of an animation to use as a thumbnail image.

