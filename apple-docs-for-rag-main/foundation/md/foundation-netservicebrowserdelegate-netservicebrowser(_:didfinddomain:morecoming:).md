

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowser(\_:didFindDomain:moreComing:) 

Instance Method

# netServiceBrowser(\_:didFindDomain:moreComing:)

Tells the delegate the sender found a domain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowser(
    _ browser: NetServiceBrowser,
    didFindDomain domainString: String,
    moreComing: Bool
)
```

## Parameters 

`browser`  

Sender of this delegate message.

`domainString`  

Name of the domain found by `netServiceBrowser`.

`moreComing`  

true when `netServiceBrowser` is waiting for additional domains. false when there are no additional domains.

## Discussion

The delegate uses this message to compile a list of available domains. It should wait until `moreDomainsComing` is false to do a bulk update of user interface elements.

## See Also

### Related Documentation

func searchForBrowsableDomains()

Initiates a search for domains visible to the host. This method returns immediately.

Deprecated

Bonjour Overview

NSNetServices and CFNetServices Programming Guide

func searchForRegistrationDomains()

Initiates a search for domains in which the host may register services.

Deprecated

### Using Network Service Browsers

func netServiceBrowser(NetServiceBrowser, didRemoveDomain: String, moreComing: Bool)

Tells the delegate the a domain has disappeared or has become unavailable.

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

