

- PDFKit
- PDFDocument
-  exchangePage(at:withPageAt:) 

Instance Method

# exchangePage(at:withPageAt:)

Swaps one page with another.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func exchangePage(
    at indexA: Int,
    withPageAt indexB: Int
)
```

## Discussion

This method raises an exception if either `index` value is out of bounds.

## See Also

### Working with Pages

var pageCount: Int

The number of pages in the document.

func page(at: Int) -> PDFPage?

Returns the page at the specified index number.

func index(for: PDFPage) -> Int

Gets the index number for the specified page.

func insert(PDFPage, at: Int)

Inserts a page at the specified index point.

func removePage(at: Int)

Removes the page at the specified index point.

var pageClass: AnyClass

The class that is allocated and initialized when page objects are created for the document.

