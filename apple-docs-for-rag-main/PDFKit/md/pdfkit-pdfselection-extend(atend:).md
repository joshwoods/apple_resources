

- PDFKit
- PDFSelection
-  extend(atEnd:) 

Instance Method

# extend(atEnd:)

Extends the selection from its end toward the end of the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func extend(atEnd succeed: Int)
```

## Discussion

The selection may be extended by any amount, up to and including the end of the document.

## See Also

### Modifying a Selection

func add(PDFSelection)

Adds the specified selection to the receiving selection.

func add([PDFSelection])

Adds the specified array of selections to the receiving selection.

func extend(atStart: Int)

Extends the selection from its start toward the beginning of the document.

