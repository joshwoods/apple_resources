

- SwiftUI
- NSHostingView
-  insertText(\_:) 

Instance Method

# insertText(\_:)

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func insertText(_ insertString: Any)
```

## See Also

### Managing keyboard interaction

func keyDown(with: NSEvent)

Called when the user presses a key on the keyboard while this view is in the responder chain.

func keyUp(with: NSEvent)

Called when the user releases a key on the keyboard while this view is in the responder chain.

func performKeyEquivalent(with: NSEvent) -> Bool

func didChangeValue(forKey: String)

func makeTouchBar() -> NSTouchBar?

