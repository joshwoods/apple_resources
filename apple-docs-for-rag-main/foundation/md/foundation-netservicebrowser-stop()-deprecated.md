

- Foundation
- NetServiceBrowser
-  stop() Deprecated

Instance Method

# stop()

Halts a currently running search or resolution.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
func stop()
```

Deprecated

Use nw_browser_t in Network framework instead

## Discussion

This method sends a netServiceBrowserDidStopSearch(_:) message to the delegate and causes the browser to discard any pending search results.

## See Also

### Related Documentation

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

### Using Network Service Browsers

func searchForBrowsableDomains()

Initiates a search for domains visible to the host. This method returns immediately.

Deprecated

func searchForRegistrationDomains()

Initiates a search for domains in which the host may register services.

Deprecated

func searchForServices(ofType: String, inDomain: String)

Starts a search for services of a particular type within a specific domain.

Deprecated

