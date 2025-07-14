

- Network
- NWProtocolFramer
- NWProtocolFramer.Instance
-  passThroughInput() 

Instance Method

# passThroughInput()

Indicates that your protocol no longer needs to handle input data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final func passThroughInput()
```

## See Also

### Delivering Input

func parseInput(minimumIncompleteLength: Int, maximumLength: Int, parse: (UnsafeMutableRawBufferPointer?, Bool) -> Int) -> Bool

Examines the content of input data while in your input handler.

func deliverInput(data: Data, message: NWProtocolFramer.Message, isComplete: Bool)

Delivers an inbound message containing arbitrary data from your protocol to the application.

func deliverInputNoCopy(length: Int, message: NWProtocolFramer.Message, isComplete: Bool) -> Bool

Delivers an inbound message containing a specific number of next received bytes.

