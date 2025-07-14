

- PDFKit
- PDFPage
-  selectionForWord(at:) 

Instance Method

# selectionForWord(at:)

Returns the whole word that includes the specified point.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
func selectionForWord(at point: NSPoint) -> PDFSelection?
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func selectionForWord(at point: CGPoint) -> PDFSelection?
```

## Discussion

Returns `NULL` if no word contains `point`.

Use this method to respond to a double-click.

## See Also

### Working with Selections

func selection(for: CGRect) -> PDFSelection?

Returns the text enclosed within the specified rectangle, expressed in page (user) coordinates.

func selectionForLine(at: CGPoint) -> PDFSelection?

Returns the whole line of text that includes the specified point.

func selection(from: CGPoint, to: CGPoint) -> PDFSelection?

Returns the text between the two specified points in page space.

func selection(for: NSRange) -> PDFSelection?

Returns the text contained within the specified range.

