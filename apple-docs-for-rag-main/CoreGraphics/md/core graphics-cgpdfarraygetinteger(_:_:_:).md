

- Core Graphics
-  CGPDFArrayGetInteger(\_:\_:\_:) 

Function

# CGPDFArrayGetInteger(\_:\_:\_:)

Returns whether an object at a given index in a PDF array is a PDF integer and, if so, retrieves that object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.3+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func CGPDFArrayGetInteger(
    _ array: CGPDFArrayRef,
    _ index: Int,
    _ value: UnsafeMutablePointer?
) -> Bool
```

## Parameters 

`array`  

A PDF array. If this parameter is not a valid PDF array, the behavior is undefined.

`index`  

The index of the value to retrieve. If the index is outside the index space of the array (`0` to `N-1`, where `N` is the count of the array), the behavior is undefined.

`value`  

On input, a pointer to a PDF integer. If the value at the specified index is a PDF integer value, then on return contains that value, otherwise the value is undefined.

## Return Value

Returns true if there is a PDF integer at the specified index, otherwise false.

## See Also

### Getting Data from a PDF Array

func CGPDFArrayGetArray(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is another PDF array and, if so, retrieves that array.

func CGPDFArrayGetBoolean(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF Boolean and, if so, retrieves that Boolean.

func CGPDFArrayGetCount(CGPDFArrayRef) -> Int

Returns the number of items in a PDF array.

func CGPDFArrayGetDictionary(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFDictionaryRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF dictionary and, if so, retrieves that dictionary.

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

