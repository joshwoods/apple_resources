

- Core Graphics
- CGPDFDocument
-  catalog 

Instance Property

# catalog

Returns the document catalog of a Core Graphics PDF document.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var catalog: CGPDFDictionaryRef? { get }
```

## Discussion

The entries in a PDF document catalog recursively describe the contents of the PDF document. You can access the contents of a PDF document catalog by calling the function catalog. For information on accessing PDF metadata, see Quartz 2D Programming Guide.

## See Also

### Examining a PDF Document

var fileIdentifier: CGPDFArrayRef?

Gets the file identifier for a PDF document.

var info: CGPDFDictionaryRef?

Gets the information dictionary for a PDF document.

var numberOfPages: Int

Returns the number of pages in a PDF document.

func getVersion(majorVersion: UnsafeMutablePointer&lt;Int32>, minorVersion: UnsafeMutablePointer&lt;Int32>)

Returns the major and minor version numbers of a Core Graphics PDF document.

func page(at: Int) -> CGPDFPage?

Returns a page from a Core Graphics PDF document.

