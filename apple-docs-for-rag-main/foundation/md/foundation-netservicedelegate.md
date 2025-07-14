

- Foundation
-  NetServiceDelegate 

Protocol

# NetServiceDelegate

The interface a net service uses to inform its delegate about the state of the service it offers.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
protocol NetServiceDelegate : NSObjectProtocol
```

## Overview

The NetServiceDelegate protocol defines the optional methods implemented by delegates of NetService objects.

## Topics

### Using Network Services

func netServiceWillPublish(NetService)

Notifies the delegate that the network is ready to publish the service.

func netService(NetService, didNotPublish: [String : NSNumber])

Notifies the delegate that a service could not be published.

func netServiceDidPublish(NetService)

Notifies the delegate that a service was successfully published.

func netServiceWillResolve(NetService)

Notifies the delegate that the network is ready to resolve the service.

func netService(NetService, didNotResolve: [String : NSNumber])

Informs the delegate that an error occurred during resolution of a given service.

func netServiceDidResolveAddress(NetService)

Informs the delegate that the address for a given service was resolved.

func netService(NetService, didUpdateTXTRecord: Data)

Notifies the delegate that the TXT record for a given service has been updated.

func netServiceDidStop(NetService)

Informs the delegate that a publish() or resolve(withTimeout:) request was stopped.

### Accepting Connections

func netService(NetService, didAcceptConnectionWith: InputStream, outputStream: OutputStream)

Called when a client connects to a service managed by Bonjour.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Local Network Services

class NetService

A network service that broadcasts its availability using multicast DNS.

Deprecated

NSBonjourServices

Bonjour service types browsed by the app.

NSLocalNetworkUsageDescription

A message that tells the user why the app is requesting access to the local network.

