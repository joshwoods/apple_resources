

- UIKit
- UITextInput
-  firstRect(for:) 

Instance Method

# firstRect(for:)

Returns the first rectangle that encloses a range of text in a document.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func firstRect(for range: UITextRange) -> CGRect
```

**Required**

## Parameters 

`range`  

An object that represents a range of text in a document.

## Return Value

The first rectangle in a `range` of text. You might use this rectangle to draw a correction rectangle. The “first” in the name refers the rectangle enclosing the first line when the range encompasses multiple lines of text.

## See Also

### Related Documentation

func caretRect(for: UITextPosition) -> CGRect

Returns a rectangle to draw the caret at a specified insertion point.

**Required**

### Working with geometry and hit-testing

func closestPosition(to: CGPoint) -> UITextPosition?

Returns the position in a document that is closest to a specified point.

**Required**

func selectionRects(for: UITextRange) -> [UITextSelectionRect]

Returns an array of selection rects corresponding to the range of text.

**Required**

func closestPosition(to: CGPoint, within: UITextRange) -> UITextPosition?

Returns the position in a document that is closest to a specified point in a specified range.

**Required**

func characterRange(at: CGPoint) -> UITextRange?

Returns the character or range of characters that is at a specified point in a document.

**Required**

