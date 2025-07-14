

- Foundation
- NetServiceDelegate
-  netService(\_:didNotPublish:) 

Instance Method

# netService(\_:didNotPublish:)

Notifies the delegate that a service could not be published.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netService(
    _ sender: NetService,
    didNotPublish errorDict: [String : NSNumber]
)
```

## Parameters 

`sender`  

The service that could not be published.

`errorDict`  

A dictionary containing information about the problem. The dictionary contains the keys `NSNetServicesErrorCode` and `NSNetServicesErrorDomain`.

## Discussion

This method may be called long after a netServiceWillPublish(_:) message has been delivered to the delegate.

## See Also

### Using Network Services

func netServiceWillPublish(NetService)

Notifies the delegate that the network is ready to publish the service.

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

