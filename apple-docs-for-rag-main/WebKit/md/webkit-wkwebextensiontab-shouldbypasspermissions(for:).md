

- WebKit
- WKWebExtensionTab
-  shouldBypassPermissions(for:) 

Instance Method

# shouldBypassPermissions(for:)

Called to determine if the tab should bypass host permission checks.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func shouldBypassPermissions(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

This method allows the app to dynamically control whether a tab can bypass standard host permission checks.

