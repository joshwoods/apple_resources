

- Message UI
- MFMessageComposeViewController
-  addAttachmentURL(\_:withAlternateFilename:) 

Instance Method

# addAttachmentURL(\_:withAlternateFilename:)

Attaches a specified file to the message.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addAttachmentURL(
    _ attachmentURL: URL,
    withAlternateFilename alternateFilename: String?
) -> Bool
```

## Parameters 

`attachmentURL`  

The file URL for the attachment. Must not be `nil`.

`alternateFilename`  

If you supply a string here, the message UI uses it for the attachment. Use an alternate filename to better describe the attachment or to make the name more readable.

OK to use a `nil` value, in which case the attachment’s actual filename is displayed in the message UI.

## Return Value

true if the attachment at the specified URL was successfully added to the message, or false otherwise.

## Discussion

You can add zero or more attachments to a message before you display the message to the user. To access information about a message’s attachments, access the attachments property.

## See Also

### Managing attachments

func disableUserAttachments()

Disables the camera/attachment button in the message composition view.

var attachments: [[AnyHashable : Any]]?

Returns an array of dictionaries that describe the properties of an attachment.

func addAttachmentData(Data, typeIdentifier: String, filename: String) -> Bool

Attaches arbitrary content to the message.

let MFMessageComposeViewControllerAttachmentURL: String

The URL for the item that is attached to the message.

let MFMessageComposeViewControllerAttachmentAlternateFilename: String

The key for the alternate filename for the file-based item attached to the message.

func insertCollaborationItemProvider(NSItemProvider) -> Bool

