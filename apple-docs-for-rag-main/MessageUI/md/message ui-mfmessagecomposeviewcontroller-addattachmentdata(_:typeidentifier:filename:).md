

- Message UI
- MFMessageComposeViewController
-  addAttachmentData(\_:typeIdentifier:filename:) 

Instance Method

# addAttachmentData(\_:typeIdentifier:filename:)

Attaches arbitrary content to the message.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addAttachmentData(
    _ attachmentData: Data,
    typeIdentifier uti: String,
    filename: String
) -> Bool
```

## Parameters 

`attachmentData`  

Content in the form of an NSData object to attach to the message. Must not be `nil`.

`uti`  

A valid Uniform Type Identifier (UTI) appropriate for the attachment data. See Uniform Type Identifiers Reference. Must not be `nil`.

`filename`  

The name to present to the user, in the message UI, for the data attachment.

## Return Value

true if the attachment data was successfully added to the message, or false otherwise.

## Discussion

This method is especially useful when the attachment you want to add to a message does not have a file system representation. This can be the case, for example, for programmatically composed audiovisual content.

## See Also

### Managing attachments

func disableUserAttachments()

Disables the camera/attachment button in the message composition view.

var attachments: [[AnyHashable : Any]]?

Returns an array of dictionaries that describe the properties of an attachment.

func addAttachmentURL(URL, withAlternateFilename: String?) -> Bool

Attaches a specified file to the message.

let MFMessageComposeViewControllerAttachmentURL: String

The URL for the item that is attached to the message.

let MFMessageComposeViewControllerAttachmentAlternateFilename: String

The key for the alternate filename for the file-based item attached to the message.

func insertCollaborationItemProvider(NSItemProvider) -> Bool

