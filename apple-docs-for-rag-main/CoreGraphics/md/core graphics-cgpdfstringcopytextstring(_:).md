

- Core Graphics
-  CGPDFStringCopyTextString(\_:) 

Function

# CGPDFStringCopyTextString(\_:)

Returns a CFString object that represents a PDF string as a text string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFStringCopyTextString(_ string: CGPDFStringRef) -> CFString?
```

## Parameters 

`string`  

A PDF string. If this value is `NULL`, it will cause an error.

## Return Value

Returns a CFString object that represents the specified PDF string as a text string. You are responsible for releasing this object.

## See Also

### Converting PDF Strings

func CGPDFStringCopyDate(CGPDFStringRef) -> CFDate?

Converts a string to a date.

