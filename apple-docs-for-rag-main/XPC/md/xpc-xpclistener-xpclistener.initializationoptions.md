

- XPC
- XPCListener
-  XPCListener.InitializationOptions 

Structure

# XPCListener.InitializationOptions

Options that control the listener’s configuration, such as if it’s inactive at creation.

Mac Catalyst 17.0+macOS 14.0+

``` source
struct InitializationOptions
```

## Topics

### Listener creation options

static var inactive: XPCListener.InitializationOptions

Indicates that the listener isn’t activated during its creation.

static var none: XPCListener.InitializationOptions

Indicates that the listener uses a default configuration during creation.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Creating a listener

init(service: String, targetQueue: DispatchQueue?, options: XPCListener.InitializationOptions, incomingSessionHandler: (XPCListener.IncomingSessionRequest) -> XPCListener.IncomingSessionRequest.Decision) throws

Creates the server side of an XPC service using the specified service name.

class IncomingSessionRequest

A session request from a client that you accept or reject.

