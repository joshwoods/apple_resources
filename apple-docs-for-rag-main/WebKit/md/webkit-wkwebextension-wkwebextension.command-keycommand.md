

- WebKit
- WKWebExtension
- WKWebExtension.Command
-  keyCommand 

Instance Property

# keyCommand

A key command representation of the web extension command for use in the responder chain.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+visionOS 2.4+

``` source
@NSCopying @MainActor
var keyCommand: UIKeyCommand? { get }
```

## Discussion

Provides a UIKeyCommand instance representing the web extension command, ready for integration in the app.

The property is `nil` if no shortcut is defined. Otherwise, the key command is fully configured with the necessary input key and modifier flags to perform the associated command upon activation. It can be included in a view controller or other responder’s keyCommands property, enabling keyboard activation and discoverability of the web extension command.

