

- Message UI
- MFMailComposeViewController
-  setSubject(\_:) 

Instance Method

# setSubject(\_:)

Sets the initial text for the subject line of the email.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setSubject(_ subject: String)
```

## Parameters 

`subject`  

The text to display in the subject line.

## Discussion

This method replaces the previous subject text with the new text. Only call this method before you display the mail composition interface. Don’t call it after presenting the interface to the user.

## See Also

### Setting mail fields programmatically

func setToRecipients([String]?)

Sets the initial recipients to include in the email’s To field.

func setCcRecipients([String]?)

Sets the initial recipients to include in the email’s Cc field.

func setBccRecipients([String]?)

Sets the initial recipients to include in the email’s Bcc field.

func setMessageBody(String, isHTML: Bool)

Sets the initial body text to include in the email.

func addAttachmentData(Data, mimeType: String, fileName: String)

Adds the specified data as an attachment to the message.

func setPreferredSendingEmailAddress(String)

Sets the preferred email address to use in the From field, if such an address is available.

