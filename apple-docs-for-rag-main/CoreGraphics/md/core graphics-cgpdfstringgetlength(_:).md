

- Core Graphics
-  CGPDFStringGetLength(\_:) 

Function

# CGPDFStringGetLength(\_:)

Returns the number of bytes in a PDF string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFStringGetLength(_ string: CGPDFStringRef) -> Int
```

## Parameters 

`string`  

A PDF string.

## Return Value

Returns the number of bytes referenced by the string, or `0` if the string is `NULL`.

## See Also

### Getting PDF String Data

func CGPDFStringGetBytePtr(CGPDFStringRef) -> UnsafePointer&lt;UInt8>?

Returns a pointer to the bytes of a PDF string.

