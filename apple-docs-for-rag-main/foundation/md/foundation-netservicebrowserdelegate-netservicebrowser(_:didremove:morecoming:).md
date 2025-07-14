

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowser(\_:didRemove:moreComing:) 

Instance Method

# netServiceBrowser(\_:didRemove:moreComing:)

Tells the delegate a service has disappeared or has become unavailable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowser(
    _ browser: NetServiceBrowser,
    didRemove service: NetService,
    moreComing: Bool
)
```

## Parameters 

`browser`  

Sender of this delegate message.

`service`  

Network service that has become unavailable.

`moreComing`  

true when `netServiceBrowser` is waiting for additional services. false when there are no additional services.

## Discussion

The delegate uses this message to compile a list of unavailable services. It should wait until `moreServicesComing` is false to do a bulk update of user interface elements.

## See Also

### Using Network Service Browsers

func netServiceBrowser(NetServiceBrowser, didFindDomain: String, moreComing: Bool)

Tells the delegate the sender found a domain.

func netServiceBrowser(NetServiceBrowser, didRemoveDomain: String, moreComing: Bool)

Tells the delegate the a domain has disappeared or has become unavailable.

func netServiceBrowser(NetServiceBrowser, didFind: NetService, moreComing: Bool)

Tells the delegate the sender found a service.

func netServiceBrowserWillSearch(NetServiceBrowser)

Tells the delegate that a search is commencing.

func netServiceBrowser(NetServiceBrowser, didNotSearch: [String : NSNumber])

Tells the delegate that a search was not successful.

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

