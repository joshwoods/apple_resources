

- Core Graphics
-  CGPDFStreamGetDictionary(\_:) 

Function

# CGPDFStreamGetDictionary(\_:)

Returns the dictionary associated with a PDF stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFStreamGetDictionary(_ stream: CGPDFStreamRef) -> CGPDFDictionaryRef?
```

## Parameters 

`stream`  

A PDF stream.

## Return Value

The PDF dictionary for the specified stream.

## See Also

### Getting Data from a PDF Stream

func CGPDFStreamCopyData(CGPDFStreamRef, UnsafeMutablePointer&lt;CGPDFDataFormat>) -> CFData?

Returns the data associated with a PDF stream.

