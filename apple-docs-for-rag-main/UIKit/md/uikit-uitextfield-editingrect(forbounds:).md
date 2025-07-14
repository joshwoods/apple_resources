

- UIKit
- UITextField
-  editingRect(forBounds:) 

Instance Method

# editingRect(forBounds:)

Returns the rectangle for displaying editable text.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func editingRect(forBounds bounds: CGRect) -> CGRect
```

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The computed editing rectangle for the text.

## Discussion

You should not call this method directly. If you want to provide a different editing rectangle for the text, you can override this method and return that rectangle. By default, this method returns a region in the text field that is not occupied by any overlay views.

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

func clearButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the built-in Clear button.

func leftViewRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle of the text field’s left overlay view.

func rightViewRect(forBounds: CGRect) -> CGRect

Returns the drawing location of the text field’s right overlay view.

