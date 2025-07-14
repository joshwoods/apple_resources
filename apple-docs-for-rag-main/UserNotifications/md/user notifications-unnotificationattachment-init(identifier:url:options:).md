

- User Notifications
- UNNotificationAttachment
-  init(identifier:url:options:) 

Initializer

# init(identifier:url:options:)

Creates an attachment object from the specified file and options.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.14+visionOS 1.0+watchOS 3.0+

``` source
convenience init(
    identifier: String,
    url URL: URL,
    options: [AnyHashable : Any]? = nil
) throws
```

## Parameters 

`identifier`  

The unique identifier of the attachment. Use this string to identify the attachment later. If you specify an empty string, this method creates a unique identifier string for you.

`URL`  

The URL of the file you want to attach to the notification. The URL must be a file URL and the file must be readable by the current process. This parameter must not be `nil`. For a list of supported file types, see Supported File Types.

`options`  

A dictionary of options related to the attached file. Use the options to specify meta information about the attachment, such as the clipping rectangle to use for the resulting thumbnail.

## Return Value

An attachment object containing information about the specified file or `nil` if the attachment could not be created.

## Discussion

This method verifies that the specified file is readable and that the file format is one of the supported types. When errors occur, the method provides an appropriate `error` object.

When you schedule a notification request containing the attachment, the system moves the attachment’s file to a new location to facilitate access by the appropriate processes. After the move, the only way to access the file is using the methods of the UNUserNotificationCenter object.

## See Also

### Creating an Attachment

let UNNotificationAttachmentOptionsTypeHintKey: String

A hint about an attachment’s file type.

let UNNotificationAttachmentOptionsThumbnailHiddenKey: String

A Boolean value indicating whether the system hides the attachment’s thumbnail.

let UNNotificationAttachmentOptionsThumbnailClippingRectKey: String

The clipping rectangle for a thumbnail image.

let UNNotificationAttachmentOptionsThumbnailTimeKey: String

The frame number of an animation to use as a thumbnail image.

