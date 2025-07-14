

- Message UI
- MFMailComposeViewController
-  setMessageBody(\_:isHTML:) 

Instance Method

# setMessageBody(\_:isHTML:)

Sets the initial body text to include in the email.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setMessageBody(
    _ body: String,
    isHTML: Bool
)
```

## Parameters 

`body`  

The initial body text of the message. The text is interpreted as either plain text or HTML, depending on the value of the `isHTML` parameter.

`isHTML`  

Specify true if the body parameter contains HTML content or specify false if it contains plain text.

## Discussion

This method replaces the previous body content with the new content. If the user has a signature file, the body content is inserted immediately before the signature. If you want to include images with your content, you must attach the images separately using the addAttachmentData(_:mimeType:fileName:) method.

Only call this method before you display the mail composition interface. Don’t call it after presenting the interface to the user.

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

func addAttachmentData(Data, mimeType: String, fileName: String)

Adds the specified data as an attachment to the message.

func setPreferredSendingEmailAddress(String)

Sets the preferred email address to use in the From field, if such an address is available.

