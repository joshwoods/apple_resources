

- XPC
- XPCSession
-  XPCSession.InitializationOptions 

Structure

# XPCSession.InitializationOptions

Options that control the session’s configuration.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
struct InitializationOptions
```

## Topics

### Session creation options

static var inactive: XPCSession.InitializationOptions

Indicates that the session isn’t activated during its creation.

static var privileged: XPCSession.InitializationOptions

Indicates that the Mach service is in the priviledged Mach bootstrap.

static var none: XPCSession.InitializationOptions

Indicates that the listener uses a default configuration during creation.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

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

func setTargetQueue(DispatchQueue)

Sets the target dispatch queue on an inactive session for processing messages.

