

- Core Graphics
-  CGPDFScannerGetContentStream(\_:) 

Function

# CGPDFScannerGetContentStream(\_:)

Returns the content stream associated with a PDF scanner object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFScannerGetContentStream(_ scanner: CGPDFScannerRef) -> CGPDFContentStreamRef
```

## Parameters 

`scanner`  

The scanner object whose content stream you want to obtain.

## Return Value

The content stream associated with `scanner`.

## See Also

### Parsing Content

func CGPDFScannerScan(CGPDFScannerRef) -> Bool

Parses the content stream of a PDF scanner object.

