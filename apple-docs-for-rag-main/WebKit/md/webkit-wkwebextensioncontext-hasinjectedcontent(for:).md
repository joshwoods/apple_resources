

- WebKit
- WKWebExtensionContext
-  hasInjectedContent(for:) 

Instance Method

# hasInjectedContent(for:)

Checks if the extension has script or stylesheet content that can be injected into the specified URL.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func hasInjectedContent(for url: URL) -> Bool
```

## Parameters 

`url`  

The webpage URL to check.

## Return Value

Returns `YES` if the extension has content that can be injected by matching the URL against the extension’s requested match patterns.

## Discussion

The extension context will still need to be loaded and have granted website permissions for its content to actually be injected.

