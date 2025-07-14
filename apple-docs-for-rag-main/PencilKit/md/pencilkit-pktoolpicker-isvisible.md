

- PencilKit
- PKToolPicker
-  isVisible 

Instance Property

# isVisible

A Boolean value that indicates whether the tool picker is currently visible.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var isVisible: Bool { get }
```

## See Also

### Coordinating the visibility of the picker

func setVisible(Bool, forFirstResponder: UIResponder)

Sets the visibility for the tool picker, based on when the specified responder object becomes active.

func frameObscured(in: UIView) -> CGRect

Returns the portion of the specified view that the tool picker obscures.

