

- InputMethodKit
- IMKCandidates
-  setDismissesAutomatically(\_:) 

Instance Method

# setDismissesAutomatically(\_:)

Sets the state of the flag that determines whether the candidates window dismisses automatically.

macOS 10.5+

``` source
@MainActor
func setDismissesAutomatically(_ flag: Bool)
```

## Parameters 

`flag`  

true to have the candidates window dismiss automatically; otherwise false.

## Discussion

By default, if the user presses the Return or Enter keys, the candidates are dismissed and a `candidateSelected:` message is sent to the input controller. You can call the `setDismissesAutomatically:` method, passing false as the `flag` parameter to change the default dismissal behavior. The input controller still receives a `candidatesSelected:` message.

When you set the flag to false, an input method processes text input while dynamically updating the content of the candidates as the user inputs text. When a session deactivates, candidate window is hidden regardless of the state of the flag.

## See Also

### Managing Window Visibility and Behavior

func show(IMKCandidatesLocationHint)

Shows the candidates window.

func hide()

Hides a candidates window, if it is visible.

func isVisible() -> Bool

Returns whether or not the candidates window is visible.

func dismissesAutomatically() -> Bool

Returns the state of the flag that determines whether the candidates window dismisses automatically.

func update()

Updates the candidates that are displayed in the candidates window.

