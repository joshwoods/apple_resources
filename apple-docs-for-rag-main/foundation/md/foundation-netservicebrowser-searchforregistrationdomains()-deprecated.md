

- Foundation
- NetServiceBrowser
-  searchForRegistrationDomains() Deprecated

Instance Method

# searchForRegistrationDomains()

Initiates a search for domains in which the host may register services.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func searchForRegistrationDomains()
```

Deprecated

Use nw_browser_t in Network framework instead

## Discussion

This method returns immediately, sending a netServiceBrowserWillSearch(_:) message to the delegate if the network was ready to initiate the search. The delegate receives a subsequent netServiceBrowser(_:didFindDomain:moreComing:) message for each domain discovered.

Most network service browser clients do not have to use this method—it is sufficient to publish a service with the empty string, which registers it in any available registration domains automatically.

## See Also

### Related Documentation

func netServiceBrowserWillSearch(NetServiceBrowser)

Tells the delegate that a search is commencing.

func netServiceBrowser(NetServiceBrowser, didFindDomain: String, moreComing: Bool)

Tells the delegate the sender found a domain.

### Using Network Service Browsers

func searchForBrowsableDomains()

Initiates a search for domains visible to the host. This method returns immediately.

Deprecated

func searchForServices(ofType: String, inDomain: String)

Starts a search for services of a particular type within a specific domain.

Deprecated

func stop()

Halts a currently running search or resolution.

Deprecated

