

- Core Graphics
-  CGPDFArrayGetCount(\_:) 

Function

# CGPDFArrayGetCount(\_:)

Returns the number of items in a PDF array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFArrayGetCount(_ array: CGPDFArrayRef) -> Int
```

## Parameters 

`array`  

A PDF array. If this parameter is not a valid PDF array, the behavior is undefined.

## Return Value

Returns the number of items in the array.

## See Also

### Getting Data from a PDF Array

func CGPDFArrayGetArray(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is another PDF array and, if so, retrieves that array.

func CGPDFArrayGetBoolean(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF Boolean and, if so, retrieves that Boolean.

func CGPDFArrayGetDictionary(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFDictionaryRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF dictionary and, if so, retrieves that dictionary.

func CGPDFArrayGetInteger(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFInteger>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF integer and, if so, retrieves that object.

func CGPDFArrayGetName(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF name reference (represented as a constant C string) and, if so, retrieves that name.

func CGPDFArrayGetNull(CGPDFArrayRef, Int) -> Bool

Returns whether an object at a given index in a Quartz PDF array is a PDF null.

func CGPDFArrayGetNumber(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFReal>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF number and, if so, retrieves that object.

func CGPDFArrayGetObject(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFObjectRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF object and, if so, retrieves that object.

func CGPDFArrayGetStream(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFStreamRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF stream and, if so, retrieves that stream.

func CGPDFArrayGetString(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFStringRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF string and, if so, retrieves that string.

