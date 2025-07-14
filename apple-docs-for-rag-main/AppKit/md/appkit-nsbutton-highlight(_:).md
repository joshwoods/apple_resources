

- AppKit
- NSButton
-  highlight(\_:) 

Instance Method

# highlight(\_:)

Highlights (or unhighlights) the button.

macOS

``` source
@MainActor
func highlight(_ flag: Bool)
```

## Parameters 

`flag`  

true to highlight the button; false to unhighlight the button. If the current state of the button matches `flag`, no action is taken.

## Discussion

Highlighting makes the button appear recessed, displays its alternate title or image, or causes the button to appear illuminated.

## See Also

### Related Documentation

func setButtonType(NSButton.ButtonType)

Sets the button’s type, which affects its user interface and behavior when clicked.

### Managing Button State

var allowsMixedState: Bool

A Boolean value that indicates whether the button allows a mixed state.

var state: NSControl.StateValue

The button’s state.

func setNextState()

Sets the button to its next state.

