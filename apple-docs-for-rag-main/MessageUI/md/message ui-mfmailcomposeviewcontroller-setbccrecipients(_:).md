

- Message UI
- MFMailComposeViewController
-  setBccRecipients(\_:) 

Instance Method

# setBccRecipients(\_:)

Sets the initial recipients to include in the email’s Bcc field.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setBccRecipients(_ bccRecipients: [String]?)
```

## Parameters 

`bccRecipients`  

An array of String objects, each containing the email address of a single recipient.

## Discussion

This method replaces the previous blind carbon-copy (Bcc) recipients with the new ones listed in the `bccRecipients` parameter. This method doesn’t filter out duplicate email addresses, so if duplicates are present, the recipient may receive multiple copies of the email message.

Only call this method before you display the mail composition interface. Don’t call it after presenting the interface to the user.

Important

MFMailComposeViewController ignores calls to this method in Mac apps built with Mac Catalyst.

## See Also

### Setting mail fields programmatically

func setSubject(String)

Sets the initial text for the subject line of the email.

func setToRecipients([String]?)

Sets the initial recipients to include in the email’s To field.

func setCcRecipients([String]?)

Sets the initial recipients to include in the email’s Cc field.

func setMessageBody(String, isHTML: Bool)

Sets the initial body text to include in the email.

func addAttachmentData(Data, mimeType: String, fileName: String)

Adds the specified data as an attachment to the message.

func setPreferredSendingEmailAddress(String)

Sets the preferred email address to use in the From field, if such an address is available.

