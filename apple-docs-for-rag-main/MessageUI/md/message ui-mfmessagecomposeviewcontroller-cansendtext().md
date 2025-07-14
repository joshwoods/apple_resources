

- Message UI
- MFMessageComposeViewController
-  canSendText() 

Type Method

# canSendText()

Returns a Boolean value that indicates whether the current device is capable of sending text messages.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func canSendText() -> Bool
```

## Return Value

true if the device can send text messages or false if it cannot.

## Discussion

Always call this method before attempting to present the message compose view controller. A device may be unable to send messages if it does not support messaging or if it is not currently configured to send messages. This method applies only to the ability to send text messages via iMessage, SMS, and MMS.

To be notified of changes in the availability of sending text messages, register as an observer of the MFMessageComposeViewControllerTextMessageAvailabilityDidChange notification.

## See Also

### Determining if message composition is available

class func canSendAttachments() -> Bool

Indicates whether or not messages can include attachments.

class func canSendSubject() -> Bool

Indicates whether or not messages can include subject lines, according to the user’s configuration in Settings.

class func isSupportedAttachmentUTI(String) -> Bool

Indicates whether or not the message can accept a file, with the specified UTI, as an attachment.

