

- AppKit
- NSPopUpButton
-  init(frame:pullsDown:) 

Initializer

# init(frame:pullsDown:)

Returns an `NSPopUpButton` object initialized to the specified dimensions.

macOS

``` source
@MainActor
init(
    frame buttonFrame: NSRect,
    pullsDown flag: Bool
)
```

## Parameters 

`buttonFrame`  

The frame rectangle for the button, specified in the parent view’s coordinate system.

`flag`  

true if you want the receiver to display a pull-down menu; otherwise, false if you want it to display a pop-up menu.

## Return Value

An initialized `NSPopUpButton` object, or `nil` if the object could not be initialized.

## See Also

### Related Documentation

Application Menu and Pop-up List Programming Topics

var pullsDown: Bool

A Boolean value indicating whether the button displays a pull-down or pop-up menu.

