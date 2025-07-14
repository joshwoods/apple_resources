

- PencilKit
- PKToolPicker
-  frameObscured(in:) 

Instance Method

# frameObscured(in:)

Returns the portion of the specified view that the tool picker obscures.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func frameObscured(in view: UIView) -> CGRect
```

## Parameters 

`view`  

The view that’s potentially obscured by the tool picker’s palette.

## Return Value

The portion of `view` (in its own coordinate space) obscured by the palette.

## Discussion

Because the palette is transparent in places, part of your view’s content may continue to show through in the specified rectangle.

## See Also

### Coordinating the visibility of the picker

func setVisible(Bool, forFirstResponder: UIResponder)

Sets the visibility for the tool picker, based on when the specified responder object becomes active.

var isVisible: Bool

A Boolean value that indicates whether the tool picker is currently visible.

