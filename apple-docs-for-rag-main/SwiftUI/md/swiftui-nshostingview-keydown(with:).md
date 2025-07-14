

- SwiftUI
- NSHostingView
-  keyDown(with:) 

Instance Method

# keyDown(with:)

Called when the user presses a key on the keyboard while this view is in the responder chain.

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func keyDown(with event: NSEvent)
```

## See Also

### Managing keyboard interaction

func keyUp(with: NSEvent)

Called when the user releases a key on the keyboard while this view is in the responder chain.

func performKeyEquivalent(with: NSEvent) -> Bool

func insertText(Any)

func didChangeValue(forKey: String)

func makeTouchBar() -> NSTouchBar?

