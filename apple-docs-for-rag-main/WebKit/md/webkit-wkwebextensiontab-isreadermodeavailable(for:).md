

- WebKit
- WKWebExtensionTab
-  isReaderModeAvailable(for:) 

Instance Method

# isReaderModeAvailable(for:)

Called to check if reader mode is available for the tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func isReaderModeAvailable(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `NO` if not implemented.

## See Also

### Related Documentation

func isReaderModeActive(for: WKWebExtensionContext) -> Bool

Called to check if the tab is currently showing reader mode.

