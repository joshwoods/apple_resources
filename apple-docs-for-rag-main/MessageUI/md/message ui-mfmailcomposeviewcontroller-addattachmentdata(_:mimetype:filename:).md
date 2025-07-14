

- Message UI
- MFMailComposeViewController
-  addAttachmentData(\_:mimeType:fileName:) 

Instance Method

# addAttachmentData(\_:mimeType:fileName:)

Adds the specified data as an attachment to the message.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addAttachmentData(
    _ attachment: Data,
    mimeType: String,
    fileName filename: String
)
```

## Parameters 

`attachment`  

The data to attach. Typically, this is the contents of a file that you want to include. This parameter must not be `nil`.

`mimeType`  

The MIME type of the specified data. (For example, the MIME type for a JPEG image is `image/jpeg`.) For a list of valid MIME types, see http://www.iana.org/assignments/media-types/. This parameter must not be `nil`.

`filename`  

The preferred filename to associate with the data. This is the default name applied to the file when it is transferred to its destination. Any path separator (`/`) characters in the filename are converted to underscore (`_`) characters prior to transmission. This parameter must not be `nil`.

## Discussion

This method attaches the specified data after the message body, but before the user’s signature. You may attach multiple files (using different file names), but must do so prior to displaying the mail composition interface. Don’t call this method after presenting the interface to the user.

## See Also

### Setting mail fields programmatically

func setSubject(String)

Sets the initial text for the subject line of the email.

func setToRecipients([String]?)

Sets the initial recipients to include in the email’s To field.

func setCcRecipients([String]?)

Sets the initial recipients to include in the email’s Cc field.

func setBccRecipients([String]?)

Sets the initial recipients to include in the email’s Bcc field.

func setMessageBody(String, isHTML: Bool)

Sets the initial body text to include in the email.

func setPreferredSendingEmailAddress(String)

Sets the preferred email address to use in the From field, if such an address is available.

