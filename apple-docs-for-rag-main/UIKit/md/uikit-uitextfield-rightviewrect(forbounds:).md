

- UIKit
- UITextField
-  rightViewRect(forBounds:) 

Instance Method

# rightViewRect(forBounds:)

Returns the drawing location of the text field’s right overlay view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func rightViewRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The rectangle in which to draw the right overlay view.

## Discussion

You should not call this method directly. If you want to place the right overlay view in a different location, you can override this method and return the new rectangle. Note that the drawing rectangle remains unchanged in a right-to-left user interface.

## See Also

### Drawing and positioning overrides

func textRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the text field’s text.

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

