

- Foundation
- XMLParser
-  parse() 

Instance Method

# parse()

Starts the event-driven parsing operation.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func parse() -> Bool
```

## Return Value

true if the parsing operation succeeds; false if an error occurs or if the parsing operation aborts.

## See Also

### Parsing

func abortParsing()

Stops the parser object.

var parserError: (any Error)?

An NSError object from which you can obtain information about a parsing error.

