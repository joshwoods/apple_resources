

- UIKit
- UITextField
-  disabledBackground 

Instance Property

# disabledBackground

The image that represents the background appearance of the text field when it is in a disabled state.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var disabledBackground: UIImage? { get set }
```

## Discussion

Background images are drawn in the border rectangle portion of the text field. Images you use for the text field’s background should be able to stretch to fit. This property is ignored if the background property is not also set.

This property is set to `nil` by default.

## See Also

### Setting the view’s background appearance

var borderStyle: UITextField.BorderStyle

The border style for the text field.

var background: UIImage?

The image that represents the background appearance of the text field when it is in an enabled state.

