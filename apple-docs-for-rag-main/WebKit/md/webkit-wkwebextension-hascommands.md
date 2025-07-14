

- WebKit
- WKWebExtension
-  hasCommands 

Instance Property

# hasCommands

A Boolean value indicating whether the extension includes commands that users can invoke.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
var hasCommands: Bool { get }
```

## Discussion

If this property is `YES`, the extension contains one or more commands that can be performed by the user. These commands should be accessible via keyboard shortcuts, menu items, or other user interface elements provided by the app. The list of commands can be accessed via commands on an extension context, and invoked via performCommand(_:).

