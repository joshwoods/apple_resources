

- Foundation
- NetServiceDelegate
-  netServiceWillPublish(\_:) 

Instance Method

# netServiceWillPublish(\_:)

Notifies the delegate that the network is ready to publish the service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceWillPublish(_ sender: NetService)
```

## Parameters 

`sender`  

The service that is ready to publish.

## Discussion

Publication of the service proceeds asynchronously and may still generate a call to the delegate’s netService(_:didNotPublish:) method if an error occurs.

## See Also

### Related Documentation

Bonjour Overview

NSNetServices and CFNetServices Programming Guide

### Using Network Services

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

