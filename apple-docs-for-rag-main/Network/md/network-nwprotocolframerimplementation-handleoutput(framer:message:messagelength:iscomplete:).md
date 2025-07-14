

- Network
- NWProtocolFramerImplementation
-  handleOutput(framer:message:messageLength:isComplete:) 

Instance Method

# handleOutput(framer:message:messageLength:isComplete:)

Notifies your protocol about a new outbound message.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func handleOutput(
    framer: NWProtocolFramer.Instance,
    message: NWProtocolFramer.Message,
    messageLength: Int,
    isComplete: Bool
)
```

**Required**

## Parameters 

`framer`  

The framer instance associated with the connection.

`message`  

The framer message passed by the application.

`messageLength`  

The length of the message content being sent.

`isComplete`  

A boolean indicating if this the last chunk of a message.

## Discussion

The output handler is your opportunity to encapsulate or encode a signle application message. You should write any output using writeOutput(data:) or writeOutputNoCopy(length:) before returning from the output handler. If you do not write a message, the application message will be discarded.

## See Also

### Handling Data

func handleInput(framer: NWProtocolFramer.Instance) -> Int

Notifies your protocol that new inbound data is available to parse.

**Required**

