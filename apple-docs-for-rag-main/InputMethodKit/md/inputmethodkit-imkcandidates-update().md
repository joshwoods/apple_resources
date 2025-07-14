

- InputMethodKit
- IMKCandidates
-  update() 

Instance Method

# update()

Updates the candidates that are displayed in the candidates window.

macOS 10.5+

``` source
@MainActor
func update()
```

## Discussion

When you call this method, the Input Method Kit calls the candidates method of the IMKInputController class. Note that the candidates list is updated, but the visible state of the window does not change. In other words, if the window is hidden, it remains hidden. If the window is visible, it remains visible.

## See Also

### Managing Window Visibility and Behavior

func show(IMKCandidatesLocationHint)

Shows the candidates window.

func hide()

Hides a candidates window, if it is visible.

func isVisible() -> Bool

Returns whether or not the candidates window is visible.

func setDismissesAutomatically(Bool)

Sets the state of the flag that determines whether the candidates window dismisses automatically.

func dismissesAutomatically() -> Bool

Returns the state of the flag that determines whether the candidates window dismisses automatically.

