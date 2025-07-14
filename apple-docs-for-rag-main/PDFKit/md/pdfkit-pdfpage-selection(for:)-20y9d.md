

- PDFKit
- PDFPage
-  selection(for:) 

Instance Method

# selection(for:)

Returns the text contained within the specified range.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func selection(for range: NSRange) -> PDFSelection?
```

## Discussion

This method raises an exception if the range length is `0` or if either end of the range is outside the range of characters on the page.

## See Also

### Working with Selections

func selection(for: CGRect) -> PDFSelection?

Returns the text enclosed within the specified rectangle, expressed in page (user) coordinates.

func selectionForWord(at: CGPoint) -> PDFSelection?

Returns the whole word that includes the specified point.

func selectionForLine(at: CGPoint) -> PDFSelection?

Returns the whole line of text that includes the specified point.

func selection(from: CGPoint, to: CGPoint) -> PDFSelection?

Returns the text between the two specified points in page space.

