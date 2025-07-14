

- Foundation
- NetServiceDelegate
-  netService(\_:didNotResolve:) 

Instance Method

# netService(\_:didNotResolve:)

Informs the delegate that an error occurred during resolution of a given service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netService(
    _ sender: NetService,
    didNotResolve errorDict: [String : NSNumber]
)
```

## Parameters 

`sender`  

The service that did not resolve.

`errorDict`  

A dictionary containing information about the problem. The dictionary contains the keys errorCode and errorDomain.

## Discussion

Clients may try to resolve again upon receiving this error. For example, a DNS rotary may yield different IP addresses on different resolution requests. A common error condition is that no addresses were resolved during the timeout period specified in resolve(withTimeout:).

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

func netServiceDidResolveAddress(NetService)

Informs the delegate that the address for a given service was resolved.

func netService(NetService, didUpdateTXTRecord: Data)

Notifies the delegate that the TXT record for a given service has been updated.

func netServiceDidStop(NetService)

Informs the delegate that a publish() or resolve(withTimeout:) request was stopped.

