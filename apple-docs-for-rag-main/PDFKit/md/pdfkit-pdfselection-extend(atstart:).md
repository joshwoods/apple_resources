

- PDFKit
- PDFSelection
-  extend(atStart:) 

Instance Method

# extend(atStart:)

Extends the selection from its start toward the beginning of the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func extend(atStart precede: Int)
```

## Discussion

The selection may be extended by any amount, up to and including the beginning of the document.

## See Also

### Modifying a Selection

func add(PDFSelection)

Adds the specified selection to the receiving selection.

func add([PDFSelection])

Adds the specified array of selections to the receiving selection.

func extend(atEnd: Int)

Extends the selection from its end toward the end of the document.

