

- Foundation
- XMLParser
-  abortParsing() 

Instance Method

# abortParsing()

Stops the parser object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func abortParsing()
```

## Discussion

If you invoke this method, the delegate, if it implements parser(_:parseErrorOccurred:), is informed of the cancelled parsing operation.

## See Also

### Parsing

func parse() -> Bool

Starts the event-driven parsing operation.

var parserError: (any Error)?

An NSError object from which you can obtain information about a parsing error.

