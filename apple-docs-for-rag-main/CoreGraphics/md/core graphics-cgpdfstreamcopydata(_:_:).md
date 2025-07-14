

- Core Graphics
-  CGPDFStreamCopyData(\_:\_:) 

Function

# CGPDFStreamCopyData(\_:\_:)

Returns the data associated with a PDF stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFStreamCopyData(
    _ stream: CGPDFStreamRef,
    _ format: UnsafeMutablePointer
) -> CFData?
```

## Parameters 

`stream`  

A PDF stream.

`format`  

On return, contains a constant that specifies the format of the data returned—CGPDFDataFormat.raw, CGPDFDataFormat.jpegEncoded, or CGPDFDataFormat.JPEG2000.

## Return Value

A CFData object that contains a copy of the stream data. You are responsible for releasing this object.

## See Also

### Getting Data from a PDF Stream

func CGPDFStreamGetDictionary(CGPDFStreamRef) -> CGPDFDictionaryRef?

Returns the dictionary associated with a PDF stream.

