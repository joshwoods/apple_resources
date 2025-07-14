

- UIKit
- UITextInput
-  caretRect(for:) 

Instance Method

# caretRect(for:)

Returns a rectangle to draw the caret at a specified insertion point.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func caretRect(for position: UITextPosition) -> CGRect
```

**Required**

## Parameters 

`position`  

An object that identifies a location in a text input area.

## Return Value

A rectangle that defines the area for drawing the caret.

## Discussion

The system uses this value to calculate the length of the beam—the vertical line representing the pointer—when using a trackpad to interact with a text input area. You must implement this method even if text never becomes editable, and an insertion point caret never appears.

## See Also

### Related Documentation

func firstRect(for: UITextRange) -> CGRect

Returns the first rectangle that encloses a range of text in a document.

**Required**

case verticalBeam(length: CGFloat)

The pointer morphs into a vertical beam using the specified length.

### Providing the caret layout information

func caretTransform(for: UITextPosition) -> CGAffineTransform

Returns the transform to apply to the caret prior to drawing.

