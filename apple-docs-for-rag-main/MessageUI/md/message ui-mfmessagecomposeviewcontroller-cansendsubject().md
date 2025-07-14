

- Message UI
- MFMessageComposeViewController
-  canSendSubject() 

Type Method

# canSendSubject()

Indicates whether or not messages can include subject lines, according to the user’s configuration in Settings.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func canSendSubject() -> Bool
```

## Return Value

true if the device can include subject lines in messages, or false otherwise.

## See Also

### Determining if message composition is available

class func canSendText() -> Bool

Returns a Boolean value that indicates whether the current device is capable of sending text messages.

class func canSendAttachments() -> Bool

Indicates whether or not messages can include attachments.

class func isSupportedAttachmentUTI(String) -> Bool

Indicates whether or not the message can accept a file, with the specified UTI, as an attachment.

