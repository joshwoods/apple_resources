

- UIKit
- UITextInput
-  selectionRects(for:) 

Instance Method

# selectionRects(for:)

Returns an array of selection rects corresponding to the range of text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func selectionRects(for range: UITextRange) -> [UITextSelectionRect]
```

**Required**

## Parameters 

`range`  

An object representing a range in a document’s text.

## Return Value

An array of UITextSelectionRect objects that encompass the selection.

## See Also

### Working with geometry and hit-testing

func firstRect(for: UITextRange) -> CGRect

Returns the first rectangle that encloses a range of text in a document.

**Required**

func closestPosition(to: CGPoint) -> UITextPosition?

Returns the position in a document that is closest to a specified point.

**Required**

func closestPosition(to: CGPoint, within: UITextRange) -> UITextPosition?

Returns the position in a document that is closest to a specified point in a specified range.

**Required**

func characterRange(at: CGPoint) -> UITextRange?

Returns the character or range of characters that is at a specified point in a document.

**Required**

