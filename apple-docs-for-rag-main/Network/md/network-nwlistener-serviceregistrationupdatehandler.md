

- Network
- NWListener
-  serviceRegistrationUpdateHandler 

Instance Property

# serviceRegistrationUpdateHandler

A handler that receives updates for the service endpoint being advertised.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
@preconcurrency
final var serviceRegistrationUpdateHandler: ((NWListener.ServiceRegistrationChange) -> Void)? { get set }
```

## See Also

### Advertising Bonjour Services

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

var service: NWListener.Service?

A Bonjour service that advertises the listener on the local network.

struct Service

A description used to advertise the Bonjour service that a listener provides.

enum ServiceRegistrationChange

Changes to how a network listener’s service is advertised.

