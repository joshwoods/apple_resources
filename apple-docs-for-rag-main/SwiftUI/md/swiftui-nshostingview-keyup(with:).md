

- SwiftUI
- NSHostingView
-  keyUp(with:) 

Instance Method

# keyUp(with:)

Called when the user releases a key on the keyboard while this view is in the responder chain.

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func keyUp(with event: NSEvent)
```

## See Also

### Managing keyboard interaction

func keyDown(with: NSEvent)

Called when the user presses a key on the keyboard while this view is in the responder chain.

func performKeyEquivalent(with: NSEvent) -> Bool

func insertText(Any)

func didChangeValue(forKey: String)

func makeTouchBar() -> NSTouchBar?

