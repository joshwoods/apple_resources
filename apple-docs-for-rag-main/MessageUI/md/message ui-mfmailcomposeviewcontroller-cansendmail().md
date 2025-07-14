

- Message UI
- MFMailComposeViewController
-  canSendMail() 

Type Method

# canSendMail()

Returns a Boolean that indicates whether the current device is able to send email.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func canSendMail() -> Bool
```

## Return Value

true if the device is configured for sending email or false if it is not.

## Discussion

You should call this method before attempting to display the mail composition interface. If it returns false, you must not display the mail composition interface.

