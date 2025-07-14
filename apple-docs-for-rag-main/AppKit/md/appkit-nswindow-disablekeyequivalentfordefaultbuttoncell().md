

- AppKit
- NSWindow
-  disableKeyEquivalentForDefaultButtonCell() 

Instance Method

# disableKeyEquivalentForDefaultButtonCell()

Disables the default button cell’s key equivalent, so it doesn’t perform a click when the user presses Return (or Enter).

macOS

``` source
@MainActor
func disableKeyEquivalentForDefaultButtonCell()
```

## See Also

### Managing Default Buttons

var defaultButtonCell: NSButtonCell?

The button cell that performs as if clicked when the window receives a Return (or Enter) key event.

func enableKeyEquivalentForDefaultButtonCell()

Reenables the default button cell’s key equivalent, so it performs a click when the user presses Return (or Enter).

