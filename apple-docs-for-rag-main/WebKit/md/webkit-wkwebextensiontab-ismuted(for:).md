

- WebKit
- WKWebExtensionTab
-  isMuted(for:) 

Instance Method

# isMuted(for:)

Called to check if the tab is currently muted.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
optional func isMuted(for context: WKWebExtensionContext) -> Bool
```

## Parameters 

`context`  

The context in which the web extension is running.

## Discussion

Defaults to `NO` if not implemented.

## See Also

### Related Documentation

func setMuted(Bool, for: WKWebExtensionContext, completionHandler: ((any Error)?) -> Void)

Called to set the mute state of the tab.

