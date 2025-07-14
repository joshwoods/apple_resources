

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  deliverInput(data:message:isComplete:) 

Instance Method

# deliverInput(data:message:isComplete:)

Delivers an inbound message containing arbitrary data from your protocol to the application.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func deliverInput(
    data: Data,
    message: NWProtocolFramer.Message,
    isComplete: Bool
)
```

## See Also

### Delivering Input

func parseInput(minimumIncompleteLength: Int, maximumLength: Int, parse: (UnsafeMutableRawBufferPointer?, Bool) -> Int) -> Bool

Examines the content of input data while in your input handler.

func deliverInputNoCopy(length: Int, message: NWProtocolFramer.Message, isComplete: Bool) -> Bool

Delivers an inbound message containing a specific number of next received bytes.

func passThroughInput()

Indicates that your protocol no longer needs to handle input data.

