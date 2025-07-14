

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowserWillSearch(\_:) 

Instance Method

# netServiceBrowserWillSearch(\_:)

Tells the delegate that a search is commencing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowserWillSearch(_ browser: NetServiceBrowser)
```

## Parameters 

`browser`  

Sender of this delegate message.

## Discussion

This message is sent to the delegate only if the underlying network layer is ready to begin a search. The delegate can use this notification to prepare its data structures to receive data.

## See Also

### Using Network Service Browsers

func netServiceBrowser(NetServiceBrowser, didFindDomain: String, moreComing: Bool)

Tells the delegate the sender found a domain.

func netServiceBrowser(NetServiceBrowser, didRemoveDomain: String, moreComing: Bool)

Tells the delegate the a domain has disappeared or has become unavailable.

func netServiceBrowser(NetServiceBrowser, didFind: NetService, moreComing: Bool)

Tells the delegate the sender found a service.

func netServiceBrowser(NetServiceBrowser, didRemove: NetService, moreComing: Bool)

Tells the delegate a service has disappeared or has become unavailable.

func netServiceBrowser(NetServiceBrowser, didNotSearch: [String : NSNumber])

Tells the delegate that a search was not successful.

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

