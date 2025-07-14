

- UIKit
- UITextField
-  clearButtonRect(forBounds:) 

Instance Method

# clearButtonRect(forBounds:)

Returns the drawing rectangle for the built-in Clear button.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func clearButtonRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The rectangle in which to draw the clear button.

## Discussion

You should not call this method directly. If you want to place the clear button in a different location, you can override this method and return the new rectangle. Your method should call the `super` implementation and modify the returned rectangle’s origin only. Changing the size of the clear button may cause unnecessary distortion of the button image.

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

func leftViewRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle of the text field’s left overlay view.

func rightViewRect(forBounds: CGRect) -> CGRect

Returns the drawing location of the text field’s right overlay view.

