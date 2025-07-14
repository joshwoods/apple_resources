

- Core Foundation
-  kCFXMLTreeErrorLocation 

Global Variable

# kCFXMLTreeErrorLocation

Dictionary key whose value is a CFNumber containing the byte location where the error was detected.

macOS

``` source
let kCFXMLTreeErrorLocation: CFString!
```

## See Also

### Constants

let kCFXMLTreeErrorDescription: CFString!

Dictionary key whose value is a CFString containing a readable description of the error.

let kCFXMLTreeErrorLineNumber: CFString!

Dictionary key whose value is a CFNumber containing the line number where the error was detected. This may not be the line number where the actual XML error is located.

let kCFXMLTreeErrorStatusCode: CFString!

Dictionary key whose value is a CFNumber containing the error status code. See CFXMLParser for possible status code values.

