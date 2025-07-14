

- Message UI
- MFMessageComposeViewController
-  attachments 

Instance Property

# attachments

Returns an array of dictionaries that describe the properties of an attachment.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var attachments: [[AnyHashable : Any]]? { get }
```

## Discussion

Each attachment is described by an NSDictionary object in the `attachments` array. To retrieve the alternate file name for an attachment from its dictionary, use the MFMessageComposeViewControllerAttachmentAlternateFilename key.

## See Also

### Managing attachments

func disableUserAttachments()

Disables the camera/attachment button in the message composition view.

func addAttachmentURL(URL, withAlternateFilename: String?) -> Bool

Attaches a specified file to the message.

func addAttachmentData(Data, typeIdentifier: String, filename: String) -> Bool

Attaches arbitrary content to the message.

let MFMessageComposeViewControllerAttachmentURL: String

The URL for the item that is attached to the message.

let MFMessageComposeViewControllerAttachmentAlternateFilename: String

The key for the alternate filename for the file-based item attached to the message.

func insertCollaborationItemProvider(NSItemProvider) -> Bool

