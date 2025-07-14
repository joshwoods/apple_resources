

- Foundation
- NetServiceBrowser
-  searchForServices(ofType:inDomain:) Deprecated

Instance Method

# searchForServices(ofType:inDomain:)

Starts a search for services of a particular type within a specific domain.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func searchForServices(
    ofType type: String,
    inDomain domainString: String
)
```

Deprecated

Use nw_browser_t in Network framework instead

## Parameters 

`type`  

Type of the service to search for.

`domainString`  

Domain name in which to perform the search.

## Discussion

This method returns immediately, sending a netServiceBrowserWillSearch(_:) message to the delegate if the network was ready to initiate the search.The delegate receives subsequent netServiceBrowser(_:didFind:moreComing:) messages for each service discovered.

The `serviceType` argument must contain both the service type and transport layer information. To ensure that the mDNS responder searches for services, rather than hosts, make sure to prefix both the service name and transport layer name with an underscore character (”\_”). For example, to search for an HTTP service on TCP, you would use the type string “`_http._tcp.`”. Note that the period character at the end is required.

The `domainName` argument can be an explicit domain name, the generic local domain `@"local."` (note trailing period, which indicates an absolute name), or the empty string (`@""`), which indicates the default registration domains. Usually, you pass in an empty string. Note that it is acceptable to use an empty string for the `domainName` argument when publishing or browsing a service, but do not rely on this for resolution.

## See Also

### Related Documentation

func netServiceBrowser(NetServiceBrowser, didFind: NetService, moreComing: Bool)

Tells the delegate the sender found a service.

func netServiceBrowserWillSearch(NetServiceBrowser)

Tells the delegate that a search is commencing.

### Using Network Service Browsers

func searchForBrowsableDomains()

Initiates a search for domains visible to the host. This method returns immediately.

Deprecated

func searchForRegistrationDomains()

Initiates a search for domains in which the host may register services.

Deprecated

func stop()

Halts a currently running search or resolution.

Deprecated

