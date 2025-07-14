

- Message UI
- MFMessageComposeViewController
-  body 

Instance Property

# body

The initial content of the message.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var body: String? { get set }
```

## Discussion

If you want to provide initial content in the body of a message, do so before you display it. After the message is displayed you cannot change the value of this property.

## See Also

### Setting the initial message information

var recipients: [String]?

An array of strings that contains the initial recipients of the message.

var subject: String?

The initial subject of the message.

var message: MSMessage?

A message object from your iMessage app extension.

