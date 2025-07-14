

- XPC
- XPCSession
-  init(machService:targetQueue:options:incomingMessageHandler:cancellationHandler:) 

Initializer

# init(machService:targetQueue:options:incomingMessageHandler:cancellationHandler:)

Establishes a connection to a launch agent or launch daemon with the name and received message handler you specify.

Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
convenience init(
    machService: String,
    targetQueue: DispatchQueue? = nil,
    options: XPCSession.InitializationOptions = .none,
    incomingMessageHandler: ((XPCReceivedMessage) -> (any Encodable)?)? = nil,
    cancellationHandler: ((XPCRichError) -> Void)? = nil
) throws
```

## Parameters 

`machService`  

The name of the Mach service to connect to. The service name must exist in the Mach bootstrap accessible to the process and advertised in a `launchd.plist`.

`targetQueue`  

The dispatch queue to use for session events. You can specify a concurrent dispatch queue. If you specify Nil, the session uses `DISPATCH_TARGET_QUEUE_DEFAULT`.

`options`  

Attributes the session uses when establishing the connection.

`incomingMessageHandler`  

A closure the system calls when a client initiates a connection to the server.

`cancellationHandler`  

A closure the system calls when it cancels a session.

## Discussion

If the service isn’t found or is unavailable, the connection fails and this method throws an error.

By default, this method activates the session it creates and the session is ready to accept messages. To create an inactive session, specify inactive in the `options` parameter.

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

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, incomingMessageHandler: ((XPCDictionary) -> XPCDictionary?)?, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name and dictionary message handler you specify.

convenience init(machService: String, targetQueue: DispatchQueue?, options: XPCSession.InitializationOptions, cancellationHandler: ((XPCRichError) -> Void)?) throws

Establishes a connection to a launch agent or launch daemon with the name you specify.

struct InitializationOptions

Options that control the session’s configuration.

func setTargetQueue(DispatchQueue)

Sets the target dispatch queue on an inactive session for processing messages.

