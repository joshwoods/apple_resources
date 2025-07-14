

- PDFKit
- PDFSelection
-  add(\_:) 

Instance Method

# add(\_:)

Adds the specified selection to the receiving selection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func add(_ selection: PDFSelection)
```

## Discussion

Selections do not have to be contiguous. If the selection to be added overlaps with the receiving selection, the overlap is removed in a process called normalization.

## See Also

### Modifying a Selection

func add([PDFSelection])

Adds the specified array of selections to the receiving selection.

func extend(atEnd: Int)

Extends the selection from its end toward the end of the document.

func extend(atStart: Int)

Extends the selection from its start toward the beginning of the document.

