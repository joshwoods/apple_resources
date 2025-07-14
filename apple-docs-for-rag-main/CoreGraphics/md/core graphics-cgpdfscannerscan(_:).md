

- Core Graphics
-  CGPDFScannerScan(\_:) 

Function

# CGPDFScannerScan(\_:)

Parses the content stream of a PDF scanner object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFScannerScan(_ scanner: CGPDFScannerRef) -> Bool
```

## Parameters 

`scanner`  

The scanner object whose content stream you want to parse.

## Return Value

true if the entire stream is parsed successfully; false if parsing fails (for example, if the stream data is corrupted).

## Discussion

The function CGPDFScannerScan(_:) parses the PDF content stream associated with the scanner. Each time Core Graphics parses a PDF operator for which you register a callback, Core Graphics invokes your callback.

## See Also

### Parsing Content

func CGPDFScannerGetContentStream(CGPDFScannerRef) -> CGPDFContentStreamRef

Returns the content stream associated with a PDF scanner object.

