

- AppKit
- NSApplication
-  unhide(\_:) 

Instance Method

# unhide(\_:)

Restores hidden windows to the screen and makes the receiver active.

macOS

``` source
@MainActor
func unhide(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent the command.

## Discussion

Invokes unhideWithoutActivation().

## See Also

### Related Documentation

func activate(ignoringOtherApps: Bool)

Makes the receiver the active app.

Deprecated

### Hiding Windows

var isHidden: Bool

A Boolean value indicating whether the app is hidden.

func hide(Any?)

Hides all the receiver’s windows, and the next app in line is activated.

func unhideWithoutActivation()

Restores hidden windows without activating their owner (the receiver).

