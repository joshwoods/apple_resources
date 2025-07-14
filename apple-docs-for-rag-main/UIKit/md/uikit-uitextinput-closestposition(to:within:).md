

- UIKit
- UITextInput
-  closestPosition(to:within:) 

Instance Method

# closestPosition(to:within:)

Returns the position in a document that is closest to a specified point in a specified range.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func closestPosition(
    to point: CGPoint,
    within range: UITextRange
) -> UITextPosition?
```

**Required**

## Parameters 

`point`  

A point in the view that is drawing a document’s text.

`range`  

An object representing a range in a document’s text.

## Return Value

An object representing the character position in `range` that is closest to `point`.

## See Also

### Working with geometry and hit-testing

func firstRect(for: UITextRange) -> CGRect

Returns the first rectangle that encloses a range of text in a document.

**Required**

func closestPosition(to: CGPoint) -> UITextPosition?

Returns the position in a document that is closest to a specified point.

**Required**

func selectionRects(for: UITextRange) -> [UITextSelectionRect]

Returns an array of selection rects corresponding to the range of text.

**Required**

func characterRange(at: CGPoint) -> UITextRange?

Returns the character or range of characters that is at a specified point in a document.

**Required**

