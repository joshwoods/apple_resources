

- Message UI
- MFMessageComposeViewController
-  recipients 

Instance Property

# recipients

An array of strings that contains the initial recipients of the message.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var recipients: [String]? { get set }
```

## Discussion

If you want to provide an initial array of one or more recipients for a message, do so before you display it. After the message is displayed you cannot change the value of this property.

Each string in the array should contain the phone number of the intended recipient.

## See Also

### Setting the initial message information

var subject: String?

The initial subject of the message.

var body: String?

The initial content of the message.

var message: MSMessage?

A message object from your iMessage app extension.

