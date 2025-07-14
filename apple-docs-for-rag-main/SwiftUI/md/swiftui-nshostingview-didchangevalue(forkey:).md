

- SwiftUI
- NSHostingView
-  didChangeValue(forKey:) 

Instance Method

# didChangeValue(forKey:)

macOS 10.15+

``` source
@MainActor @preconcurrency
override dynamic func didChangeValue(forKey key: String)
```

## See Also

### Managing keyboard interaction

func keyDown(with: NSEvent)

Called when the user presses a key on the keyboard while this view is in the responder chain.

func keyUp(with: NSEvent)

Called when the user releases a key on the keyboard while this view is in the responder chain.

func performKeyEquivalent(with: NSEvent) -> Bool

func insertText(Any)

func makeTouchBar() -> NSTouchBar?

