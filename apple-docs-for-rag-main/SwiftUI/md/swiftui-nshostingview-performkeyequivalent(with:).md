

- SwiftUI
- NSHostingView
-  performKeyEquivalent(with:) 

Instance Method

# performKeyEquivalent(with:)

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func performKeyEquivalent(with nsEvent: NSEvent) -> Bool
```

## See Also

### Managing keyboard interaction

func keyDown(with: NSEvent)

Called when the user presses a key on the keyboard while this view is in the responder chain.

func keyUp(with: NSEvent)

Called when the user releases a key on the keyboard while this view is in the responder chain.

func insertText(Any)

func didChangeValue(forKey: String)

func makeTouchBar() -> NSTouchBar?

