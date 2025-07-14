

- InputMethodKit
- IMKCandidates
-  show(\_:) 

Instance Method

# show(\_:)

Shows the candidates window.

macOS 10.5+

``` source
@MainActor
func show(_ locationHint: IMKCandidatesLocationHint)
```

## Parameters 

`locationHint`  

A IMKCandidatesLocationHint constant that specifies the desired position of the candidates window. The Input Method Kit uses the hint to place the candidates window in a location that is in the vicinity of the hint location and ensures that the candidates window is fully visible.

## Discussion

Your input method calls this method when it is appropriate during text conversion to display a list of candidates.

## See Also

### Managing Window Visibility and Behavior

func hide()

Hides a candidates window, if it is visible.

func isVisible() -> Bool

Returns whether or not the candidates window is visible.

func setDismissesAutomatically(Bool)

Sets the state of the flag that determines whether the candidates window dismisses automatically.

func dismissesAutomatically() -> Bool

Returns the state of the flag that determines whether the candidates window dismisses automatically.

func update()

Updates the candidates that are displayed in the candidates window.

