

- Core Graphics
-  CGPDFOperatorTable 

API Collection

# CGPDFOperatorTable

A set of callback functions for operators used when scanning content in a PDF document.

## Overview

You pass an operator table and a PDF content stream to a CGPDFScanner object. When the scanner parses a PDF operator, Core Graphics invokes your callback for that operator. See also CGPDFScanner and CGPDFContentStream.

Note

This object is not derived from CFType and therefore you can’t use the Core Foundation base functions on it, such as CFRetain and CFRelease. In Objective-C, handle memory management with CGPDFOperatorTableRetain(_:) and CGPDFOperatorTableRelease(_:).

For more about PDF operators, see the latest version of *PDF Reference*, Adobe Systems Incorporated.

## Topics

### Creating a PDF Operator Table

func CGPDFOperatorTableCreate() -> CGPDFOperatorTableRef?

Creates an empty PDF operator table.

### Setting Callback Functions

func CGPDFOperatorTableSetCallback(CGPDFOperatorTableRef, UnsafePointer&lt;CChar>, CGPDFOperatorCallback)

Sets a callback function for a PDF operator.

### Retaining and Releasing a PDF Operator Table

func CGPDFOperatorTableRetain(CGPDFOperatorTableRef) -> CGPDFOperatorTableRef

Increments the retain count of a CGPDFOperatorTable object.

func CGPDFOperatorTableRelease(CGPDFOperatorTableRef)

Decrements the retain count of a CGPDFOperatorTable object.

### Callbacks

typealias CGPDFOperatorCallback

Performs custom processing for PDF operators.

### Data Types

typealias CGPDFOperatorTableRef

A type that stores callback functions for PDF operators.

