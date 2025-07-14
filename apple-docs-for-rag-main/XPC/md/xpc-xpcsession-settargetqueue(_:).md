

- XPC
- XPCSession
-  setTargetQueue(\_:) 

Instance Method

# setTargetQueue(\_:)

Sets the target dispatch queue on an inactive session for processing messages.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
func setTargetQueue(_ targetQueue: DispatchQueue)
```

## Parameters 

`targetQueue`  

The dispatch queue where the session processes messages. The target queue can be a concurrent queue.

## See Also

### Creating a session

convenience init&lt;Message>(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((Message) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name and decodable message handler you specify.

convenience init(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCReceivedMessage) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name and received message handler you specify.

convenience init(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCDictionary) -> XPCDictionary?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name and dictionary message handler you specify.

convenience init(xpcService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to an XPC service with the name you specify.

convenience init&lt;Message>(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((Message) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and decodable message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCReceivedMessage) -> (any Encodable)?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and received message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCDictionary) -> XPCDictionary?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and dictionary message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name you specify.

struct InitializationOptions

Options that control the session’s configuration.

