

- WebKit
- WKWebExtensionTab
-  isLoadingComplete(for:) 

Instance Method

# isLoadingComplete(for:)

Called to check if the tab has finished loading.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func isLoadingComplete(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to isLoading of the tab’s web view if not implemented.

