

- Foundation
- NetServiceDelegate
-  netServiceDidStop(\_:) 

Instance Method

# netServiceDidStop(\_:)

Informs the delegate that a publish() or resolve(withTimeout:) request was stopped.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceDidStop(_ sender: NetService)
```

## Parameters 

`sender`  

The service that stopped.

## See Also

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

