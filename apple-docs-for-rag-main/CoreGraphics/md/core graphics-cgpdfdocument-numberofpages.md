

- Core Graphics
- CGPDFDocument
-  numberOfPages 

Instance Property

# numberOfPages

Returns the number of pages in a PDF document.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var numberOfPages: Int { get }
```

## See Also

### Examining a PDF Document

var catalog: CGPDFDictionaryRef?

Returns the document catalog of a Core Graphics PDF document.

var fileIdentifier: CGPDFArrayRef?

Gets the file identifier for a PDF document.

var info: CGPDFDictionaryRef?

Gets the information dictionary for a PDF document.

func getVersion(majorVersion: UnsafeMutablePointer&lt;Int32>, minorVersion: UnsafeMutablePointer&lt;Int32>)

Returns the major and minor version numbers of a Core Graphics PDF document.

func page(at: Int) -> CGPDFPage?

Returns a page from a Core Graphics PDF document.

