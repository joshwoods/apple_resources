

- BrowserEngineKit
- BETextInteraction
-  refreshKeyboardUI() 

Instance Method

# refreshKeyboardUI()

Tells the system to refresh the keyboard UI.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func refreshKeyboardUI()
```

## Discussion

This lightweight method refreshes the selection UI. For example, this could be invoked in response to programmatic text selection changes, independent of text interaction gestures

## See Also

### UI updates

func editabilityChanged()

Tells the system that the document’s editability status has changed.

