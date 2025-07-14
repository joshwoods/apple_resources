

- AppKit
- NSPopUpButton
-  autoenablesItems 

Instance Property

# autoenablesItems

A Boolean value indicating whether the button enables and disables its items every time a user event occurs.

macOS

``` source
@MainActor
var autoenablesItems: Bool { get set }
```

## Discussion

When the value of this property is true, user events cause the button to enable and disable its items automatically according to the NSMenuValidation protocol specification.

## See Also

### Setting the type of menu

var pullsDown: Bool

A Boolean value indicating whether the button displays a pull-down or pop-up menu.

