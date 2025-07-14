

- Message UI
- MFMessageComposeViewController
-  subject 

Instance Property

# subject

The initial subject of the message.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var subject: String? { get set }
```

## Discussion

If you want to provide an initial subject for a message, do so before you display it. After the message is displayed you cannot change the value of this property.

## See Also

### Setting the initial message information

var recipients: [String]?

An array of strings that contains the initial recipients of the message.

var body: String?

The initial content of the message.

var message: MSMessage?

A message object from your iMessage app extension.

