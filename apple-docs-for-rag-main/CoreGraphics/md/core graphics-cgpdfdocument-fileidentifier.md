

- Core Graphics
- CGPDFDocument
-  fileIdentifier 

Instance Property

# fileIdentifier

Gets the file identifier for a PDF document.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fileIdentifier: CGPDFArrayRef? { get }
```

## Discussion

A PDF file identifier is defined in the PDF specification as an array of two strings, the first of which is a permanent identifier that doesn’t change even when the file is updated. The second string changes each time the file is updated. For more information, see *PDF Reference: Version 1.3 (Second Edition)*, Adobe Systems Incorporated.

## See Also

### Examining a PDF Document

var catalog: CGPDFDictionaryRef?

Returns the document catalog of a Core Graphics PDF document.

var info: CGPDFDictionaryRef?

Gets the information dictionary for a PDF document.

var numberOfPages: Int

Returns the number of pages in a PDF document.

func getVersion(majorVersion: UnsafeMutablePointer&lt;Int32>, minorVersion: UnsafeMutablePointer&lt;Int32>)

Returns the major and minor version numbers of a Core Graphics PDF document.

func page(at: Int) -> CGPDFPage?

Returns a page from a Core Graphics PDF document.

