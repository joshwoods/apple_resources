

- PDFKit
- PDFPage
-  selection(for:) 

Instance Method

# selection(for:)

Returns the text enclosed within the specified rectangle, expressed in page (user) coordinates.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func selection(for rect: CGRect) -> PDFSelection?
```

**macOS**

``` source
func selection(for rect: NSRect) -> PDFSelection?
```

## See Also

### Working with Selections

func selectionForWord(at: CGPoint) -> PDFSelection?

Returns the whole word that includes the specified point.

func selectionForLine(at: CGPoint) -> PDFSelection?

Returns the whole line of text that includes the specified point.

func selection(from: CGPoint, to: CGPoint) -> PDFSelection?

Returns the text between the two specified points in page space.

func selection(for: NSRange) -> PDFSelection?

Returns the text contained within the specified range.

