

- Foundation
- NetServiceDelegate
-  netService(\_:didUpdateTXTRecord:) 

Instance Method

# netService(\_:didUpdateTXTRecord:)

Notifies the delegate that the TXT record for a given service has been updated.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netService(
    _ sender: NetService,
    didUpdateTXTRecord data: Data
)
```

## Parameters 

`sender`  

The service whose TXT record was updated.

`data`  

The new TXT record.

## See Also

### Related Documentation

func startMonitoring()

Starts the monitoring of TXT-record updates for the receiver.

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

func netServiceDidResolveAddress(NetService)

Informs the delegate that the address for a given service was resolved.

func netServiceDidStop(NetService)

Informs the delegate that a publish() or resolve(withTimeout:) request was stopped.

