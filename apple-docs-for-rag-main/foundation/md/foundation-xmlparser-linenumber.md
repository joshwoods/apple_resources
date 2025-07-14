

- Foundation
- XMLParser
-  lineNumber 

Instance Property

# lineNumber

The line number of the XML document being processed by the parser.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lineNumber: Int { get }
```

## Discussion

You may access this property once a parsing operation has begun or after an error occurs.

## See Also

### Obtaining Parser State

var columnNumber: Int

The column number of the XML document being processed by the parser.

var publicID: String?

The public identifier of the external entity referenced in the XML document.

var systemID: String?

The system identifier of the external entity referenced in the XML document.

