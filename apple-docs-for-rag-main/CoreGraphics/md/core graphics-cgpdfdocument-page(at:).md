

- Core Graphics
- CGPDFDocument
-  page(at:) 

Instance Method

# page(at:)

Returns a page from a Core Graphics PDF document.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func page(at pageNumber: Int) -> CGPDFPage?
```

## Parameters 

`pageNumber`  

The number of the page requested.

## Return Value

Return the PDF page corresponding to the specified page number, or `NULL` if no such page exists in the document. Pages are numbered starting at 1.

## See Also

### Examining a PDF Document

var catalog: CGPDFDictionaryRef?

Returns the document catalog of a Core Graphics PDF document.

var fileIdentifier: CGPDFArrayRef?

Gets the file identifier for a PDF document.

var info: CGPDFDictionaryRef?

Gets the information dictionary for a PDF document.

var numberOfPages: Int

Returns the number of pages in a PDF document.

func getVersion(majorVersion: UnsafeMutablePointer&lt;Int32>, minorVersion: UnsafeMutablePointer&lt;Int32>)

Returns the major and minor version numbers of a Core Graphics PDF document.

