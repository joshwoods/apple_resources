

- Core Graphics
-  CGPDFScannerRetain(\_:) 

Function

# CGPDFScannerRetain(\_:)

Increments the retain count of a scanner object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFScannerRetain(_ scanner: CGPDFScannerRef) -> CGPDFScannerRef
```

## Parameters 

`scanner`  

The scanner object to retain.

## Return Value

The same scanner object passed to the function in the `scanner` parameter.

## See Also

### Retaining and Releasing PDF Scanner Objects

func CGPDFScannerRelease(CGPDFScannerRef)

Decrements the retain count of a scanner object.

