

- BrowserEngineKit
- BETextInteraction
-  editabilityChanged() 

Instance Method

# editabilityChanged()

Tells the system that the document’s editability status has changed.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func editabilityChanged()
```

## Discussion

In response, the system refreshes the text interaction gestures, depending on the value of `isEditable`

## See Also

### UI updates

func refreshKeyboardUI()

Tells the system to refresh the keyboard UI.

