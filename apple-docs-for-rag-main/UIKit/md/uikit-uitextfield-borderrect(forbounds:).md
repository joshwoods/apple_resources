

- UIKit
- UITextField
-  borderRect(forBounds:) 

Instance Method

# borderRect(forBounds:)

Returns the text field’s border rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func borderRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The border rectangle for the receiver.

## Discussion

You should not call this method directly. If you want to provide a different border rectangle for drawing, you can override this method and return that rectangle.

The default implementation of this method returns the original `bounds` rectangle.

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

func editingRect(forBounds: CGRect) -> CGRect

Returns the rectangle for displaying editable text.

func clearButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the built-in Clear button.

func leftViewRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle of the text field’s left overlay view.

func rightViewRect(forBounds: CGRect) -> CGRect

Returns the drawing location of the text field’s right overlay view.

