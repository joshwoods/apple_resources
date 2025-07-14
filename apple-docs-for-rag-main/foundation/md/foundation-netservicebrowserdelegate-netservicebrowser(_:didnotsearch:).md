

- Foundation
- NetServiceBrowserDelegate
-  netServiceBrowser(\_:didNotSearch:) 

Instance Method

# netServiceBrowser(\_:didNotSearch:)

Tells the delegate that a search was not successful.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
optional func netServiceBrowser(
    _ browser: NetServiceBrowser,
    didNotSearch errorDict: [String : NSNumber]
)
```

## Parameters 

`browser`  

Sender of this delegate message.

`errorDict`  

Dictionary with the reasons the search was unsuccessful. Use the dictionary keys errorCode and errorDomain to retrieve the error information from the dictionary.

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

func netServiceBrowserWillSearch(NetServiceBrowser)

Tells the delegate that a search is commencing.

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

