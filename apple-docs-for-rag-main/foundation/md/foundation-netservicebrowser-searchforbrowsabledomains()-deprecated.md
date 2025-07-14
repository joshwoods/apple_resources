

- Foundation
- NetServiceBrowser
-  searchForBrowsableDomains() Deprecated

Instance Method

# searchForBrowsableDomains()

Initiates a search for domains visible to the host. This method returns immediately.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func searchForBrowsableDomains()
```

Deprecated

Use nw_browser_t in Network framework instead

## Discussion

The delegate receives a netServiceBrowser(_:didFindDomain:moreComing:) message for each domain discovered.

## See Also

### Using Network Service Browsers

func searchForRegistrationDomains()

Initiates a search for domains in which the host may register services.

Deprecated

func searchForServices(ofType: String, inDomain: String)

Starts a search for services of a particular type within a specific domain.

Deprecated

func stop()

Halts a currently running search or resolution.

Deprecated

