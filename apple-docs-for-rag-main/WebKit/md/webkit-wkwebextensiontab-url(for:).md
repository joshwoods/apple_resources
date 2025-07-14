

- WebKit
- WKWebExtensionTab
-  url(for:) 

Instance Method

# url(for:)

Called when the URL of the tab is needed.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func url(for context: WKWebExtensionContext) -> URL?
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `URL` of the tab’s web view if not implemented.

