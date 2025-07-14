

- Core Foundation
- CFXMLTree
-  Error Dictionary Keys 

API Collection

# Error Dictionary Keys

The keys used in an error dictionary returned by some functions to provide more information about XML parse errors.

## Overview

These keys are used in the error dictionary returned by the CFXMLTreeCreateFromDataWithError function.

## Topics

### Constants

let kCFXMLTreeErrorDescription: CFString!

Dictionary key whose value is a CFString containing a readable description of the error.

let kCFXMLTreeErrorLineNumber: CFString!

Dictionary key whose value is a CFNumber containing the line number where the error was detected. This may not be the line number where the actual XML error is located.

let kCFXMLTreeErrorLocation: CFString!

Dictionary key whose value is a CFNumber containing the byte location where the error was detected.

let kCFXMLTreeErrorStatusCode: CFString!

Dictionary key whose value is a CFNumber containing the error status code. See CFXMLParser for possible status code values.

