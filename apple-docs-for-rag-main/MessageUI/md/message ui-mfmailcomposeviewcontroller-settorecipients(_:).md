

- Message UI
- MFMailComposeViewController
-  setToRecipients(\_:) 

Instance Method

# setToRecipients(\_:)

Sets the initial recipients to include in the email’s To field.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setToRecipients(_ toRecipients: [String]?)
```

## Parameters 

`toRecipients`  

An array of String objects, each containing the email address of a single recipient.

## Discussion

This method replaces the previous recipients with the new ones listed in the `toRecipients` parameter. This method doesn’t filter out duplicate email addresses, so if duplicates are present, multiple copies of the email message may be sent to the same address.

Only call this method before you display the mail composition interface. Don’t call it after presenting the interface to the user.

## See Also

### Setting mail fields programmatically

func setSubject(String)

Sets the initial text for the subject line of the email.

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

