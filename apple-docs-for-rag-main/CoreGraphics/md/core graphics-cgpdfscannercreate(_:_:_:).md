

- Core Graphics
-  CGPDFScannerCreate(\_:\_:\_:) 

Function

# CGPDFScannerCreate(\_:\_:\_:)

Creates a PDF scanner.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFScannerCreate(
    _ cs: CGPDFContentStreamRef,
    _ table: CGPDFOperatorTableRef?,
    _ info: UnsafeMutableRawPointer?
) -> CGPDFScannerRef
```

## Parameters 

`cs`  

A PDF content stream object. (See CGPDFContentStream.)

`table`  

A table of callbacks for the PDF operators you want to handle.

`info`  

A pointer to data you want passed to your callback function. (See CGPDFOperatorTable.)

## Return Value

A PDF scanner object. In Objective-C, you’re responsible for releasing this object by calling the function CGPDFScannerRelease(_:).

## Discussion

When you want to parse the contents of the PDF stream, call the function CGPDFScannerScan(_:).

