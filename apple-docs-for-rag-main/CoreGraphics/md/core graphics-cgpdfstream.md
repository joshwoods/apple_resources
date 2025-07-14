

- Core Graphics
-  CGPDFStream 

API Collection

# CGPDFStream

A stream or sequence of data bytes in a PDF document.

## Overview

A PDF stream consists of a dictionary that describes a sequence of bytes. Streams typically represent objects with potentially large amounts of data, such as images and page descriptions.

This object is not derived from CFType and therefore there are no functions for retaining and releasing it.

## Topics

### Getting Data from a PDF Stream

func CGPDFStreamCopyData(CGPDFStreamRef, UnsafeMutablePointer&lt;CGPDFDataFormat>) -> CFData?

Returns the data associated with a PDF stream.

func CGPDFStreamGetDictionary(CGPDFStreamRef) -> CGPDFDictionaryRef?

Returns the dictionary associated with a PDF stream.

### Data Types

typealias CGPDFStreamRef

A type that represents a PDF stream.

### Constants

enum CGPDFDataFormat

The encoding format of PDF data.

## See Also

### Related Documentation

Quartz 2D Programming Guide

