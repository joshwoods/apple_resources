

- PDFKit
- PDFDocument
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts a page at the specified index point.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func insert(
    _ page: PDFPage,
    at index: Int
)
```

## Discussion

This method raises an exception if `index` is out of bounds.

Be aware that a PDF viewing application might use the size of the first page in the document as representative of all page sizes when reporting the size of a document. If you need to get the actual size of an individual page, you can use bounds(for:) (note that the size is returned in points, which are typically converted to inches or centimeters by PDF viewing applications).

## See Also

### Working with Pages

var pageCount: Int

The number of pages in the document.

func page(at: Int) -> PDFPage?

Returns the page at the specified index number.

func index(for: PDFPage) -> Int

Gets the index number for the specified page.

func removePage(at: Int)

Removes the page at the specified index point.

func exchangePage(at: Int, withPageAt: Int)

Swaps one page with another.

var pageClass: AnyClass

The class that is allocated and initialized when page objects are created for the document.

