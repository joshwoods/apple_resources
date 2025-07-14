

- Core Graphics
-  CGPDFContentStreamRetain(\_:) 

Function

# CGPDFContentStreamRetain(\_:)

Increments the retain count of a PDF content stream object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFContentStreamRetain(_ cs: CGPDFContentStreamRef) -> CGPDFContentStreamRef
```

## Parameters 

`cs`  

A PDF content stream object.

## Return Value

The same PDF content stream you passed in as the `cs` parameter.

## See Also

### Retaining and Releasing a PDF Content Stream Object

func CGPDFContentStreamRelease(CGPDFContentStreamRef)

Decrements the retain count of a PDF content stream object.

