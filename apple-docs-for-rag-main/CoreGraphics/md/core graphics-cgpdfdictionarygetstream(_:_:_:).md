

- Core Graphics
-  CGPDFDictionaryGetStream(\_:\_:\_:) 

Function

# CGPDFDictionaryGetStream(\_:\_:\_:)

Returns whether there is a PDF stream associated with a specified key in a PDF dictionary and, if so, retrieves that stream.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFDictionaryGetStream(
    _ dict: CGPDFDictionaryRef,
    _ key: UnsafePointer,
    _ value: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`dict`  

A PDF dictionary. If this parameter is not a valid PDF dictionary, the behavior is undefined.

`key`  

The key for the value to be retrieved.

`value`  

On input, a pointer to a PDF stream. If the value associated with the specified key is a PDF stream, then on return contains that stream; otherwise, the value is unspecified.

## Return Value

Returns true if there is a PDF stream associated with the specified key; otherwise, false.

## See Also

### Getting Data from a Dictionary

func CGPDFDictionaryGetArray(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Returns whether there is a PDF array associated with a specified key in a PDF dictionary and, if so, retrieves that array.

func CGPDFDictionaryGetBoolean(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Returns whether there is a PDF Boolean value associated with a specified key in a PDF dictionary and, if so, retrieves the Boolean value.

func CGPDFDictionaryGetCount(CGPDFDictionaryRef) -> Int

Returns the number of entries in a PDF dictionary.

func CGPDFDictionaryGetDictionary(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFDictionaryRef?>?) -> Bool

Returns whether there is another PDF dictionary associated with a specified key in a PDF dictionary and, if so, retrieves that dictionary.

func CGPDFDictionaryGetInteger(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFInteger>?) -> Bool

Returns whether there is a PDF integer associated with a specified key in a PDF dictionary and, if so, retrieves that integer.

func CGPDFDictionaryGetName(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>?) -> Bool

Returns whether an object with a specified key in a PDF dictionary is a PDF name reference (represented as a constant C string) and, if so, retrieves that name.

func CGPDFDictionaryGetNumber(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFReal>?) -> Bool

Returns whether there is a PDF number associated with a specified key in a PDF dictionary and, if so, retrieves that number.

func CGPDFDictionaryGetObject(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFObjectRef?>?) -> Bool

Returns whether there is a PDF object associated with a specified key in a PDF dictionary and, if so, retrieves that object.

func CGPDFDictionaryGetString(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFStringRef?>?) -> Bool

Returns whether there is a PDF string associated with a specified key in a PDF dictionary and, if so, retrieves that string.

