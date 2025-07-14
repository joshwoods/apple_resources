

- UIKit
- UITextField
-  textRect(forBounds:) 

Instance Method

# textRect(forBounds:)

Returns the drawing rectangle for the text field’s text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func textRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The computed drawing rectangle for the label’s text.

## Discussion

You should not call this method directly. If you want to customize the drawing rectangle for the text, you can override this method and return a different rectangle.

The default implementation of this method returns a rectangle that is derived from the control’s original bounds, but which does not include the area occupied by the receiver’s border or overlay views.

## See Also

### Drawing and positioning overrides

func drawText(in: CGRect)

Draws the text field’s text in the specified rectangle.

Deprecated

func placeholderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the text field’s placeholder text.

func drawPlaceholder(in: CGRect)

Draws the text field’s placeholder text in the specified rectangle.

func borderRect(forBounds: CGRect) -> CGRect

Returns the text field’s border rectangle.

func editingRect(forBounds: CGRect) -> CGRect

Returns the rectangle for displaying editable text.

func clearButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the built-in Clear button.

func leftViewRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle of the text field’s left overlay view.

func rightViewRect(forBounds: CGRect) -> CGRect

Returns the drawing location of the text field’s right overlay view.

