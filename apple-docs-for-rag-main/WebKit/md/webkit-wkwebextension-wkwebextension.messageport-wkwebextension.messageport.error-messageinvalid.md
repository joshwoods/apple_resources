

- WebKit
- WKWebExtension
- WKWebExtension.MessagePort
- WKWebExtension.MessagePort.Error
-  messageInvalid 

Type Property

# messageInvalid

Indicates that the message is invalid.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
static var messageInvalid: WKWebExtension.MessagePort.Error.Code { get }
```

## Discussion

The message must be an object that is JSON-serializable.

