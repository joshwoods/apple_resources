

- Core Graphics
-  CGPDFStringCopyDate(\_:) 

Function

# CGPDFStringCopyDate(\_:)

Converts a string to a date.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.4+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFStringCopyDate(_ string: CGPDFStringRef) -> CFDate?
```

## Parameters 

`string`  

The string to convert to a date.

## Return Value

A CFDate object.

## Discussion

The PDF specification defines a specific format for strings that represent dates. This function converts strings in that form to CFDate objects.

## See Also

### Converting PDF Strings

func CGPDFStringCopyTextString(CGPDFStringRef) -> CFString?

Returns a CFString object that represents a PDF string as a text string.

