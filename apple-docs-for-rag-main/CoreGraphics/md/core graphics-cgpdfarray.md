

- Core Graphics
-  CGPDFArray 

API Collection

# CGPDFArray

An array structure within a PDF document.

## Overview

PDF arrays may be heterogeneous—that is, they may contain any other PDF objects, including PDF strings, PDF dictionaries, and other PDF arrays.

Many `CGPDFArray` functions to retrieve values from a PDF array take the form:

```
bool CGPDFArrayGet (
 CGPDFArrayRef array,
 size_t index,
 Ref *value
);
```

These functions test the data type of the object at the specified index. If the object is not of the expected type, the function returns false. If the object is of the expected type, the function returns true, and the object is passed back in the `value` parameter.

This type is not derived from CFTypeRef and therefore there are no functions for retaining and releasing it. CGPDFArrayRef objects exist only as constituent parts of a CGPDFDocument object, and they are managed by their container.

## Topics

### Getting Data from a PDF Array

func CGPDFArrayGetArray(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Returns whether an object at a given index in a PDF array is another PDF array and, if so, retrieves that array.

func CGPDFArrayGetBoolean(CGPDFArrayRef, Int, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Returns whether an object at a given index in a PDF array is a PDF Boolean and, if so, retrieves that Boolean.

func CGPDFArrayGetCount(CGPDFArrayRef) -> Int

Returns the number of items in a PDF array.

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

### Data Types

typealias CGPDFArrayRef

An opaque type that encapsulates a PDF array.

## See Also

### Related Documentation

Quartz 2D Programming Guide

