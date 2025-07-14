

- InputMethodKit
- IMKCandidates
-  hide() 

Instance Method

# hide()

Hides a candidates window, if it is visible.

macOS 10.5+

``` source
@MainActor
func hide()
```

## See Also

### Managing Window Visibility and Behavior

func show(IMKCandidatesLocationHint)

Shows the candidates window.

func isVisible() -> Bool

Returns whether or not the candidates window is visible.

func setDismissesAutomatically(Bool)

Sets the state of the flag that determines whether the candidates window dismisses automatically.

func dismissesAutomatically() -> Bool

Returns the state of the flag that determines whether the candidates window dismisses automatically.

func update()

Updates the candidates that are displayed in the candidates window.

