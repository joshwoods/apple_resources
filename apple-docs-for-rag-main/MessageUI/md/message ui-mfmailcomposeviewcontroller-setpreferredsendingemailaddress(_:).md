

- Message UI
- MFMailComposeViewController
-  setPreferredSendingEmailAddress(\_:) 

Instance Method

# setPreferredSendingEmailAddress(\_:)

Sets the preferred email address to use in the From field, if such an address is available.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setPreferredSendingEmailAddress(_ emailAddress: String)
```

## Parameters 

`emailAddress`  

The preferred email address used to send this message.

## Discussion

If the user doesn’t have an account with a preferred address set up, the default account is used instead.

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

func setMessageBody(String, isHTML: Bool)

Sets the initial body text to include in the email.

func addAttachmentData(Data, mimeType: String, fileName: String)

Adds the specified data as an attachment to the message.

