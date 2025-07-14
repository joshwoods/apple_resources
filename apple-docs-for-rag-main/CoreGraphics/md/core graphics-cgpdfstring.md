

- Core Graphics
-  CGPDFString 

API Collection

# CGPDFString

A text string in a PDF document.

## Overview

A PDF string object is a series of bytes—unsigned integer values in the range 0 to 255.

The string elements are not integer objects, but are stored in a more compact format. For more information on the representation of strings in PDF, see the latest version of *PDF Reference*, Adobe Systems Incorporated.

This object is not derived from CFType and therefore there are no functions for retaining and releasing it. CGPDFString objects exist as constituent parts of a CGPDFDocument object, and are managed by their container.

## Topics

### Converting PDF Strings

func CGPDFStringCopyTextString(CGPDFStringRef) -> CFString?

Returns a CFString object that represents a PDF string as a text string.

func CGPDFStringCopyDate(CGPDFStringRef) -> CFDate?

Converts a string to a date.

### Getting PDF String Data

func CGPDFStringGetBytePtr(CGPDFStringRef) -> UnsafePointer&lt;UInt8>?

Returns a pointer to the bytes of a PDF string.

func CGPDFStringGetLength(CGPDFStringRef) -> Int

Returns the number of bytes in a PDF string.

### Data Types

typealias CGPDFStringRef

A data type that represents a string in a PDF document.

## See Also

### Related Documentation

Quartz 2D Programming Guide

