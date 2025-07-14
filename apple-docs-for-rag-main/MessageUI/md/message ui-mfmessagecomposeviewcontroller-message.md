

- Message UI
- MFMessageComposeViewController
-  message 

Instance Property

# message

A message object from your iMessage app extension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+

``` source
@NSCopying @MainActor
var message: MSMessage? { get set }
```

## Discussion

If your app has an iMessage app extension, you can display your iMessage app within the message compose view, just as you would in the Messages app. To display your iMessage app, create and assign an MSMessage object to this property.

By default, this property is set to `nil`.

For more information on creating iMessage apps, see Messages.

## See Also

### Setting the initial message information

var recipients: [String]?

An array of strings that contains the initial recipients of the message.

var subject: String?

The initial subject of the message.

var body: String?

The initial content of the message.

