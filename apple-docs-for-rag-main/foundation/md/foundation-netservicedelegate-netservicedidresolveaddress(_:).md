

- Foundation
- NetServiceDelegate
-  netServiceDidResolveAddress(\_:) 

Instance Method

# netServiceDidResolveAddress(\_:)

Informs the delegate that the address for a given service was resolved.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceDidResolveAddress(_ sender: NetService)
```

## Parameters 

`sender`  

The service that was resolved.

## Discussion

The delegate can use the addresses method to retrieve the service’s address. If the delegate needs only one address, it can stop the resolution process using stop(). Otherwise, the resolution will continue until the timeout specified in resolve(withTimeout:) is reached.

## See Also

### Related Documentation

var addresses: [Data]?

A read-only array containing `NSData` objects, each of which contains a socket address for the service.

Deprecated

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

func netService(NetService, didUpdateTXTRecord: Data)

Notifies the delegate that the TXT record for a given service has been updated.

func netServiceDidStop(NetService)

Informs the delegate that a publish() or resolve(withTimeout:) request was stopped.

