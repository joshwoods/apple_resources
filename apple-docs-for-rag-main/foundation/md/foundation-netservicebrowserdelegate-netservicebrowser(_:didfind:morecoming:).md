

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowser(\_:didFind:moreComing:) 

Instance Method

# netServiceBrowser(\_:didFind:moreComing:)

Tells the delegate the sender found a service.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowser(
    _ browser: NetServiceBrowser,
    didFind service: NetService,
    moreComing: Bool
)
```

## Parameters 

`browser`  

Sender of this delegate message.

`service`  

Network service found by `netServiceBrowser`. The delegate can use this object to connect to and use the service.

`moreComing`  

true when `netServiceBrowser` is waiting for additional services. false when there are no additional services.

## Discussion

The delegate uses this message to compile a list of available services. It should wait until `moreServicesComing` is false to do a bulk update of user interface elements.

### Special Considerations

If the delegate chooses to resolve `netService`, it should retain `netService` and set itself as that service’s delegate. The delegate should, therefore, release that service when it receives the netServiceDidResolveAddress(_:) or netService(_:didNotResolve:) delegate messages of the NetService class.

## See Also

### Related Documentation

func searchForServices(ofType: String, inDomain: String)

Starts a search for services of a particular type within a specific domain.

Deprecated

### Using Network Service Browsers

func netServiceBrowser(NetServiceBrowser, didFindDomain: String, moreComing: Bool)

Tells the delegate the sender found a domain.

func netServiceBrowser(NetServiceBrowser, didRemoveDomain: String, moreComing: Bool)

Tells the delegate the a domain has disappeared or has become unavailable.

func netServiceBrowser(NetServiceBrowser, didRemove: NetService, moreComing: Bool)

Tells the delegate a service has disappeared or has become unavailable.

func netServiceBrowserWillSearch(NetServiceBrowser)

Tells the delegate that a search is commencing.

func netServiceBrowser(NetServiceBrowser, didNotSearch: [String : NSNumber])

Tells the delegate that a search was not successful.

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

