

- WebKit
- WKWebExtensionContext
-  commands 

Instance Property

# commands

The commands associated with the extension.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var commands: [WKWebExtension.Command] { get }
```

## Discussion

Provides all commands registered within the extension. Each command represents an action or behavior available for the web extension.

## See Also

### Related Documentation

func performCommand(WKWebExtension.Command)

Performs the specified command, triggering events specific to this extension.

