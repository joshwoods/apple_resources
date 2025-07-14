

- XPC
- XPCSession
-  send(message:replyHandler:) 

Instance Method

# send(message:replyHandler:)

Sends a message asynchronously over the session to the destination service, calling a closure after receiving a reply.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func send(
    message: XPCDictionary,
    replyHandler: @escaping (Result) -> Void
)
```

## Parameters 

`message`  

A dictionary object that contains the message to send.

`replyHandler`  

A closure the session invokes when it receives a reply. The closure takes a result parameter that contains either the reply that the destination sent back or an error describing a failure.

## Discussion

Sessions send messages serially in a first-in, first-out (FIFO) order. This method is safe to call from multiple dispatch queues. The session can’t indicate whether the message *delivery* is successful or not. While the session may successfully enqueue the message at the remote end of the connection, there’s no guarantee about when the destination dequeues the message and invokes the receiving session’s handler.

If the session fails to send the message, this method throws an error that contains details about the failure.

If the system tears down the session’s connection before receiving a reply, it invokes `replyHandler` with a result containing an XPCRichError describing the failure. For example, the remote service exits prematurely before sending a reply.

Important

If you create an inactive session, you must activate it before sending messages. Calling this method with an inactive session crashes.

## See Also

### Sending messages

func send&lt;Message>(Message) throws

Sends an encodable message over the session to the destination service.

func send&lt;Message>(Message, replyHandler: (Result&lt;XPCReceivedMessage, XPCRichError>) -> Void) throws

Sends an encodable message over the session to the destination service, using the closure you specify to handle a reply and rich error.

func send&lt;Message, Reply>(Message, replyHandler: (Result&lt;Reply, any Error>) -> Void) throws

Sends an encodable message over the session to the destination service, using the closure you specify to handle a reply.

func send(message: XPCDictionary) throws

Sends a dictionary message over the session to the destination service.

func sendSync&lt;Message>(Message) throws -> XPCReceivedMessage

Sends an encodable message over the session to the destination service, blocking the caller until receiving a reply message.

func sendSync&lt;Message, Reply>(Message) throws -> Reply

Sends an encodable message over the session to the destination service, blocking the caller until receiving an encodable reply message.

func sendSync(message: XPCDictionary) throws -> XPCDictionary

Sends a dictionary message over the session to the destination service, blocking the caller until receiving a reply.

