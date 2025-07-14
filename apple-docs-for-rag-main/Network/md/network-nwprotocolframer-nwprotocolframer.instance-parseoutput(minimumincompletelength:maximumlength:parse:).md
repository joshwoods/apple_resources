

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  parseOutput(minimumIncompleteLength:maximumLength:parse:) 

Instance Method

# parseOutput(minimumIncompleteLength:maximumLength:parse:)

Examines the content of output data while inside your output handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func parseOutput(
    minimumIncompleteLength: Int,
    maximumLength: Int,
    parse: (UnsafeMutableRawBufferPointer?, Bool) -> Int
) -> Bool
```

## Parameters 

`minimumIncompleteLength`  

The minimum number of bytes that should be delivered to the parse completion.

`maximumLength`  

The maximum number of bytes that should be delivered to the parse completion.

`parse`  

A completion handler that will be called inline to examine a region of bytes. This will contain the buffer that matches the constraints, and a boolean indicating if this buffer represents the end of a message.

## Return Value

Returns true if the requested length was available to parse, or false if the conditions could not be met.

## See Also

### Writing Output

func writeOutput(data: Data)

Sends arbitrary output data from your protocol to the next protocol.

func writeOutputNoCopy(length: Int) throws

Sends a specific number of bytes from a message while inside your output handler.

func passThroughOutput()

Indicates that your protocol no longer needs to handle output data.

