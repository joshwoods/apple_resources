

- XPC
- XPCSession
-  sendSync(\_:) 

Instance Method

# sendSync(\_:)

Sends an encodable message over the session to the destination service, blocking the caller until receiving an encodable reply message.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func sendSync(_ message: Message) throws -> Reply where Message : Encodable, Reply : Decodable
```

## Parameters 

`message`  

An encodable object that contains the message to send.

## Return Value

If successful, the response to the message; otherwise this method throws an error.

## Discussion

This method supports priority inversion avoidance. Use this method instead of calling send(message:replyHandler:) and using a semaphore.

Be judicious about your use of this API. It can block indefinitely. Calling this method while the session’s target queue is blocked may lead to deadlocks in certain scenarios. For that reason, invoking this method from the session’s target queue results in a crash.

Tip

If you provide an API that uses this method, consider allowing callers to specify a queue and callback handler to let you provide results asynchronously.

Sessions send messages serially in a first-in, first-out (FIFO) order. This method is safe to call from multiple dispatch queues. The session can’t indicate whether the message *delivery* is successful or not. While the session may successfully enqueue the message at the remote end of the connection, there’s no guarantee about when the destination dequeues the message and invokes the receiving session’s handler.

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

func send(message: XPCDictionary, replyHandler: (Result&lt;XPCDictionary, XPCRichError>) -> Void)

Sends a message asynchronously over the session to the destination service, calling a closure after receiving a reply.

func sendSync&lt;Message>(Message) throws -> XPCReceivedMessage

Sends an encodable message over the session to the destination service, blocking the caller until receiving a reply message.

func sendSync(message: XPCDictionary) throws -> XPCDictionary

Sends a dictionary message over the session to the destination service, blocking the caller until receiving a reply.

