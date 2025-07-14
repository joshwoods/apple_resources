

- PencilKit
- PKToolPicker
-  setVisible(\_:forFirstResponder:) 

Instance Method

# setVisible(\_:forFirstResponder:)

Sets the visibility for the tool picker, based on when the specified responder object becomes active.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setVisible(
    _ visible: Bool,
    forFirstResponder responder: UIResponder
)
```

## Parameters 

`visible`  

A Boolean value that indicates whether to make the palette visible when `responder` becomes active. Specify true to show the palette when the object becomes the first responder.

`responder`  

A responder object associated with the tool picker’s window. Typically, you specify a view capable of becoming the first responder.

## Discussion

Each time you call this method with the `visible` parameter set to true, the tool picker adds `responder` to a list of objects to monitor. When any object in the list becomes the first responder, the tool picker displays the palette. Calling this method with the `visible` parameter set to false removes `responder` from the list of monitored objects.

## See Also

### Coordinating the visibility of the picker

var isVisible: Bool

A Boolean value that indicates whether the tool picker is currently visible.

func frameObscured(in: UIView) -> CGRect

Returns the portion of the specified view that the tool picker obscures.

