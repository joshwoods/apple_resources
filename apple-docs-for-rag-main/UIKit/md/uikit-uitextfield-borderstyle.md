

- UIKit
- UITextField
-  borderStyle 

Instance Property

# borderStyle

The border style for the text field.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var borderStyle: UITextField.BorderStyle { get set }
```

## Discussion

The default value for this property is UITextField.BorderStyle.none. If the value is set to the UITextField.BorderStyle.roundedRect style, the custom background image associated with the text field is ignored.

## See Also

### Setting the view’s background appearance

var background: UIImage?

The image that represents the background appearance of the text field when it is in an enabled state.

var disabledBackground: UIImage?

The image that represents the background appearance of the text field when it is in a disabled state.

