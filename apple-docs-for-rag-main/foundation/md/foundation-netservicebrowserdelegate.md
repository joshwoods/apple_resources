

- Foundation
-  NetServiceBrowserDelegate 

Protocol

# NetServiceBrowserDelegate

The interface a net service browser uses to inform a delegate about the state of service discovery.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+

``` source
protocol NetServiceBrowserDelegate : NSObjectProtocol
```

## Overview

Delegates of NetServiceBrowser instances optionally implement these methods.

## Topics

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

func netServiceBrowserDidStopSearch(NetServiceBrowser)

Tells the delegate that a search was stopped.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Service Discovery

class NetServiceBrowser

A network service browser that finds published services on a network using multicast DNS.

Deprecated

