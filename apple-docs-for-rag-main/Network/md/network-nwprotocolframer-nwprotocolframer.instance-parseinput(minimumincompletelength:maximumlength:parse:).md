

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  parseInput(minimumIncompleteLength:maximumLength:parse:) 

Instance Method

# parseInput(minimumIncompleteLength:maximumLength:parse:)

Examines the content of input data while in your input handler.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func parseInput(
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

### Delivering Input

func deliverInput(data: Data, message: NWProtocolFramer.Message, isComplete: Bool)

Delivers an inbound message containing arbitrary data from your protocol to the application.

func deliverInputNoCopy(length: Int, message: NWProtocolFramer.Message, isComplete: Bool) -> Bool

Delivers an inbound message containing a specific number of next received bytes.

func passThroughInput()

Indicates that your protocol no longer needs to handle input data.

