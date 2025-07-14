

- Core Graphics
-  CGPDFObject 

API Collection

# CGPDFObject

An object representing content within a PDF document.

## Overview

PDF supports several basic types of object: Boolean values, integer and real numbers, strings, names, arrays, dictionaries, and streams. Most of these are represented in Core Graphics by corresponding specific types. A CGPDFObject can represent any of these types. You use CGPDFObject functions to determine the type of the object, and retrieve the object value if it is of an expected type.

This object is not derived from CFType and therefore there are no functions for retaining and releasing it. CGPDFObject objects exist as constituent parts of a CGPDFDocument object, and are managed by their container.

## Topics

### Getting Object Types and Values

func CGPDFObjectGetType(CGPDFObjectRef) -> CGPDFObjectType

Returns the PDF type identifier of an object.

func CGPDFObjectGetValue(CGPDFObjectRef, CGPDFObjectType, UnsafeMutableRawPointer?) -> Bool

Returns whether an object is of a given type and if it is, retrieves its value.

### Data Types

typealias CGPDFObjectRef

A type that contains information about a PDF object.

typealias CGPDFBoolean

A PDF Boolean value.

typealias CGPDFInteger

A PDF integer value.

typealias CGPDFReal

A PDF real value.

### Constants

enum CGPDFObjectType

Types of PDF object.

## See Also

### Related Documentation

Quartz 2D Programming Guide

