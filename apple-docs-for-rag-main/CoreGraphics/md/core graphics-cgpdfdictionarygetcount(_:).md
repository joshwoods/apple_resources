

- Core Graphics
-  CGPDFDictionaryGetCount(\_:) 

Function

# CGPDFDictionaryGetCount(\_:)

Returns the number of entries in a PDF dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFDictionaryGetCount(_ dict: CGPDFDictionaryRef) -> Int
```

## Parameters 

`dict`  

A PDF dictionary. If this parameter is not a valid PDF dictionary, the behavior is undefined.

## Return Value

Returns the number of entries in the dictionary.

## See Also

### Getting Data from a Dictionary

func CGPDFDictionaryGetArray(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Returns whether there is a PDF array associated with a specified key in a PDF dictionary and, if so, retrieves that array.

func CGPDFDictionaryGetBoolean(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Returns whether there is a PDF Boolean value associated with a specified key in a PDF dictionary and, if so, retrieves the Boolean value.

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

func CGPDFDictionaryGetStream(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFStreamRef?>?) -> Bool

Returns whether there is a PDF stream associated with a specified key in a PDF dictionary and, if so, retrieves that stream.

func CGPDFDictionaryGetString(CGPDFDictionaryRef, UnsafePointer&lt;CChar>, UnsafeMutablePointer&lt;CGPDFStringRef?>?) -> Bool

Returns whether there is a PDF string associated with a specified key in a PDF dictionary and, if so, retrieves that string.

