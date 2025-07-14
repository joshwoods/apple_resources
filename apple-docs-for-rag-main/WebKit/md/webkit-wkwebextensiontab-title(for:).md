

- WebKit
- WKWebExtensionTab
-  title(for:) 

Instance Method

# title(for:)

Called when the title of the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func title(for context: WKWebExtensionContext) -> String?
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to title of the tab’s web view if not implemented.

