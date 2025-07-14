

- Core Graphics
-  CGPDFScanner 

API Collection

# CGPDFScanner

A parser object for handling content and operators in a PDF content stream.

## Overview

You can set up the PDF scanner object to invoke callbacks when it encounters specific PDF operators in the stream.

This object is not derived from `CFType`. In Objective-C, use CGPDFScannerRetain(_:) and CGPDFScannerRelease(_:) to manage the retain count of CGPDFScannerRef instances; do not use CFRetain and CFRelease.

## Topics

### Creating a PDF Scanner Object

func CGPDFScannerCreate(CGPDFContentStreamRef, CGPDFOperatorTableRef?, UnsafeMutableRawPointer?) -> CGPDFScannerRef

Creates a PDF scanner.

### Retaining and Releasing PDF Scanner Objects

func CGPDFScannerRetain(CGPDFScannerRef) -> CGPDFScannerRef

Increments the retain count of a scanner object.

func CGPDFScannerRelease(CGPDFScannerRef)

Decrements the retain count of a scanner object.

### Parsing Content

func CGPDFScannerScan(CGPDFScannerRef) -> Bool

Parses the content stream of a PDF scanner object.

func CGPDFScannerGetContentStream(CGPDFScannerRef) -> CGPDFContentStreamRef

Returns the content stream associated with a PDF scanner object.

### Getting PDF Objects from the Scanner Stack

func CGPDFScannerPopObject(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFObjectRef?>?) -> Bool

Retrieves an object from the scanner stack.

func CGPDFScannerPopBoolean(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFBoolean>?) -> Bool

Retrieves a Boolean object from the scanner stack.

func CGPDFScannerPopInteger(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFInteger>?) -> Bool

Retrieves an integer object from the scanner stack.

func CGPDFScannerPopNumber(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFReal>?) -> Bool

Retrieves a real value object from the scanner stack.

func CGPDFScannerPopName(CGPDFScannerRef, UnsafeMutablePointer&lt;UnsafePointer&lt;CChar>?>?) -> Bool

Retrieves a character string from the scanner stack.

func CGPDFScannerPopString(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFStringRef?>?) -> Bool

Retrieves a string object from the scanner stack.

func CGPDFScannerPopArray(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFArrayRef?>?) -> Bool

Retrieves an array object from the scanner stack.

func CGPDFScannerPopDictionary(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFDictionaryRef?>?) -> Bool

Retrieves a PDF dictionary object from the scanner stack.

func CGPDFScannerPopStream(CGPDFScannerRef, UnsafeMutablePointer&lt;CGPDFStreamRef?>?) -> Bool

Retrieves a PDF stream object from the scanner stack.

### Data Types

typealias CGPDFScannerRef

A type used to parse a PDF content stream.

## See Also

### Related Documentation

Quartz 2D Programming Guide

