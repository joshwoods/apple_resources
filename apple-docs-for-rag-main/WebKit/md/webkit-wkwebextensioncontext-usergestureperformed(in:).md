

- WebKit
- WKWebExtensionContext
-  userGesturePerformed(in:) 

Instance Method

# userGesturePerformed(in:)

Should be called by the app when a user gesture is performed in a specific tab.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+visionOS 2.4+

``` source
@MainActor
func userGesturePerformed(in tab: any WKWebExtensionTab)
```

## Parameters 

`tab`  

The tab in which the user gesture was performed.

## Discussion

When a user gesture is performed in a tab, this method should be called to update the extension context.

This enables the extension to be aware of the user gesture, potentially granting it access to features that require user interaction, such as `activeTab`. Not required if using performAction(for:).

## See Also

### Related Documentation

func hasActiveUserGesture(in: any WKWebExtensionTab) -> Bool

Indicates if a user gesture is currently active in the specified tab.

