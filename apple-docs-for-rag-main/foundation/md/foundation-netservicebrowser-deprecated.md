

- Foundation
-  NetServiceBrowser Deprecated

Class

# NetServiceBrowser

A network service browser that finds published services on a network using multicast DNS.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
class NetServiceBrowser
```

Deprecated

Use nw_browser_t in Network framework instead

## Overview

Services can range from standard services, such as HTTP and FTP, to custom services defined by other applications. You can use a network service browser in your code to obtain the list of accessible domains and then to obtain an NetService object for each discovered service. Each network service browser performs one search at a time, so if you want to perform multiple simultaneous searches, use multiple network service browsers.

A network service browser performs all searches asynchronously using the current run loop to execute the search in the background. Results from a search are returned through the associated delegate object, which your client application must provide. Searching proceeds in the background until the object receives a stop() message.

To use an `NSNetServiceBrowser` object to search for services, allocate it, initialize it, and assign a delegate. (If you wish, you can also use the schedule(in:forMode:) and remove(from:forMode:) methods to execute searches on a run loop other than the current one.) Once your object is ready, you begin by gathering the list of accessible domains using either the searchForRegistrationDomains() or searchForBrowsableDomains() methods. From the list of returned domains, you can pick one and use the searchForServices(ofType:inDomain:) method to search for services in that domain.

The `NSNetServiceBrowser` class provides two ways to search for domains. In most cases, your client should use the searchForRegistrationDomains() method to search only for local domains to which the host machine has registration authority. This is the preferred method for accessing domains as it guarantees that the host machine can connect to services in the returned domains. Access to domains outside this list may be more limited.

## Topics

### Creating Network Service Browsers

init()

Initializes an allocated NetServiceBrowser object.

### Configuring Network Service Browsers

var delegate: (any NetServiceBrowserDelegate)?

The delegate object for this instance.

var includesPeerToPeer: Bool

Whether to browse over peer-to-peer Bluetooth and Wi-Fi, if available. false, by default.

### Using Network Service Browsers

func searchForBrowsableDomains()

Initiates a search for domains visible to the host. This method returns immediately.

func searchForRegistrationDomains()

Initiates a search for domains in which the host may register services.

func searchForServices(ofType: String, inDomain: String)

Starts a search for services of a particular type within a specific domain.

func stop()

Halts a currently running search or resolution.

### Managing Run Loops

func schedule(in: RunLoop, forMode: RunLoop.Mode)

Adds the receiver to the specified run loop.

func remove(from: RunLoop, forMode: RunLoop.Mode)

Removes the receiver from the specified run loop.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Service Discovery

protocol NetServiceBrowserDelegate

The interface a net service browser uses to inform a delegate about the state of service discovery.

