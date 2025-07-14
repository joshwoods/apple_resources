

- Network
- NWListener
-  NWListener.Service 

Structure

# NWListener.Service

A description used to advertise the Bonjour service that a listener provides.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
struct Service
```

## Topics

### Defining Services

init(name: String?, type: String, domain: String?, txtRecord: Data?)

Initializes a Bonjour service to advertise.

init(name: String?, type: String, domain: String?, txtRecord: NWTXTRecord)

Initializes a Bonjour service to advertise with a TXT record.

var noAutoRename: Bool

A Boolean that indicates whether the service prohibits automatic renaming in the event of a name conflict.

### Inspecting Services

let name: String?

The Bonjour name of the service.

let type: String

The Bonjour type of the service.

let domain: String?

The Bonjour domain of the service.

var txtRecordObject: NWTXTRecord?

The TXT record to advertise with the service.

let txtRecord: Data?

The TXT record as a raw buffer to advertise with the service.

### Initializers

init(applicationService: String)

Creates a listener for apps that listen for connections from a network device picker.

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Equatable
- Sendable

## See Also

### Advertising Bonjour Services

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

var service: NWListener.Service?

A Bonjour service that advertises the listener on the local network.

var serviceRegistrationUpdateHandler: ((NWListener.ServiceRegistrationChange) -> Void)?

A handler that receives updates for the service endpoint being advertised.

enum ServiceRegistrationChange

Changes to how a network listener’s service is advertised.

