

- Core Graphics
- CGPDFDocument
-  getVersion(majorVersion:minorVersion:) 

Instance Method

# getVersion(majorVersion:minorVersion:)

Returns the major and minor version numbers of a Core Graphics PDF document.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func getVersion(
    majorVersion: UnsafeMutablePointer,
    minorVersion: UnsafeMutablePointer
)
```

## Parameters 

`majorVersion`  

On return, contains the major version number of the document.

`minorVersion`  

On return, contains the minor version number of the document.

## Discussion

On return, the values of the `majorVersion` and `minorVersion` parameters are set to the major and minor version numbers of the document respectively.

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

func page(at: Int) -> CGPDFPage?

Returns a page from a Core Graphics PDF document.

