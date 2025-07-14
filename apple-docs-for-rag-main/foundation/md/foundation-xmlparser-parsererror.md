

- Foundation
- XMLParser
-  parserError 

Instance Property

# parserError

An NSError object from which you can obtain information about a parsing error.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var parserError: (any Error)? { get }
```

## Discussion

You may access this property after a parsing operation abnormally terminates to determine the cause of error.

## See Also

### Parsing

func parse() -> Bool

Starts the event-driven parsing operation.

func abortParsing()

Stops the parser object.

