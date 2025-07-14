

- Core Graphics
-  CGPDFStringGetBytePtr(\_:) 

Function

# CGPDFStringGetBytePtr(\_:)

Returns a pointer to the bytes of a PDF string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFStringGetBytePtr(_ string: CGPDFStringRef) -> UnsafePointer?
```

## Parameters 

`string`  

A PDF string.

## Return Value

Returns a pointer to the bytes of the specified string. If the string is `NULL`, the function returns `NULL`.

## See Also

### Getting PDF String Data

func CGPDFStringGetLength(CGPDFStringRef) -> Int

Returns the number of bytes in a PDF string.

