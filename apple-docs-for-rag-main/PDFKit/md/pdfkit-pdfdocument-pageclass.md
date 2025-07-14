

- PDFKit
- PDFDocument
-  pageClass 

Instance Property

# pageClass

The class that is allocated and initialized when page objects are created for the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var pageClass: AnyClass { get }
```

## Discussion

If you want to supply a custom page class, subclass `PDFDocument` and implement this method to return your custom class. Note that your custom class must be a subclass of PDFPage; otherwise, the behavior is undefined.

The default implementation of `pageClass` returns `[PDFPage class]`.

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

func exchangePage(at: Int, withPageAt: Int)

Swaps one page with another.

