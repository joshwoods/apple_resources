

- UIKit
- UITextField
-  drawPlaceholder(in:) 

Instance Method

# drawPlaceholder(in:)

Draws the text field’s placeholder text in the specified rectangle.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func drawPlaceholder(in rect: CGRect)
```

## Parameters 

`rect`  

The rectangle in which to draw the placeholder text.

## Discussion

You should not call this method directly. If you want to customize the drawing behavior for the placeholder text, you can override this method to do your drawing.

By the time this method is called, the current graphics context is already configured with the default environment and text color for drawing. In your overridden method, you can configure the current context further and then invoke `super` to do the actual drawing or do the drawing yourself. If you do render the text yourself, you should not invoke `super`.

## See Also

### Drawing and positioning overrides

func textRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the text field’s text.

func drawText(in: CGRect)

Draws the text field’s text in the specified rectangle.

Deprecated

func placeholderRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the text field’s placeholder text.

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

