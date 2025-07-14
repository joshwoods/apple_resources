

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowserDidStopSearch(\_:) 

Instance Method

# netServiceBrowserDidStopSearch(\_:)

Tells the delegate that a search was stopped.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowserDidStopSearch(_ browser: NetServiceBrowser)
```

## Parameters 

`browser`  

Sender of this delegate message.

## Discussion

When `netServiceBrowser` receives a stop() message from its client, `netServiceBrowser` sends a `netServiceBrowserDidStopSearch:` message to its delegate. The delegate then performs any necessary cleanup.

## See Also

### Related Documentation

func stop()

Halts a currently running search or resolution.

Deprecated

### Using Network Service Browsers

func netServiceBrowser(NetServiceBrowser, didFindDomain: String, moreComing: Bool)

Tells the delegate the sender found a domain.

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

