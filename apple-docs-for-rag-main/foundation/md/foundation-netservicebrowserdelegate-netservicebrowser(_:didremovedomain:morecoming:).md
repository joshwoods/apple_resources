

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowser(\_:didRemoveDomain:moreComing:) 

Instance Method

# netServiceBrowser(\_:didRemoveDomain:moreComing:)

Tells the delegate the a domain has disappeared or has become unavailable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowser(
    _ browser: NetServiceBrowser,
    didRemoveDomain domainString: String,
    moreComing: Bool
)
```

## Parameters 

`browser`  

Sender of this delegate message.

`domainString`  

Name of the domain that became unavailable.

`moreComing`  

true when `netServiceBrowser` is waiting for additional domains. false when there are no additional domains.

## Discussion

The delegate uses this message to compile a list of unavailable domains. It should wait until `moreDomainsComing` is false to do a bulk update of user interface elements.

## See Also

### Using Network Service Browsers

func netServiceBrowser(NetServiceBrowser, didFindDomain: String, moreComing: Bool)

Tells the delegate the sender found a domain.

func netServiceBrowser(NetServiceBrowser, didFind: NetService, moreComing: Bool)

Tells the delegate the sender found a service.

func netServiceBrowser(NetServiceBrowser, didRemove: NetService, moreComing: Bool)

Tells the delegate a service has disappeared or has become unavailable.

func netServiceBrowserWillSearch(NetServiceBrowser)

Tells the delegate that a search is commencing.

func netServiceBrowser(NetServiceBrowser, didNotSearch: [String : NSNumber])

Tells the delegate that a search was not successful.

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

