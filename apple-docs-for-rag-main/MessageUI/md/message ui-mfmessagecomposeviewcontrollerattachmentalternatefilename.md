

- Message UI
-  MFMessageComposeViewControllerAttachmentAlternateFilename 

Global Variable

# MFMessageComposeViewControllerAttachmentAlternateFilename

The key for the alternate filename for the file-based item attached to the message.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
let MFMessageComposeViewControllerAttachmentAlternateFilename: String
```

## Discussion

Use this constant with the attachments property to retrieve the optional, more descriptive name for a message attachment.

## See Also

### Managing attachments

func disableUserAttachments()

Disables the camera/attachment button in the message composition view.

var attachments: [[AnyHashable : Any]]?

Returns an array of dictionaries that describe the properties of an attachment.

func addAttachmentURL(URL, withAlternateFilename: String?) -> Bool

Attaches a specified file to the message.

func addAttachmentData(Data, typeIdentifier: String, filename: String) -> Bool

Attaches arbitrary content to the message.

let MFMessageComposeViewControllerAttachmentURL: String

The URL for the item that is attached to the message.

func insertCollaborationItemProvider(NSItemProvider) -> Bool

