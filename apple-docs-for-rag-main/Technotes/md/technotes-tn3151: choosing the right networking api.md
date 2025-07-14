

- Technotes
-  TN3151: Choosing the right networking API 

Article

# TN3151: Choosing the right networking API

Learn which networking API is best for you.

## Overview

Apple platforms have a wide range of networking APIs, spanning many different frameworks:

- Foundation

- Network

- BSD Sockets in the System framework

- And more

With all that choice, it’s hard to know where to start. This technote aims to clarify that. It makes specific recommendations as to which API to use for a given network protocol. It then discusses Alternative APIs and some Best practices.

Important

If you’re working on watchOS, read TN3135: Low-level networking on watchOS to understand its unique constraints.

The focus here is on APIs that allow you to *use* the networking stack. If you want to *extend* the networking stack—for example, to add support for a custom VPN protocol—implement a Network Extension provider. For the details, see Network Extension.

## Recommendations by protocol

This section lists API recommendations for common network protocols. Follow the advice for the protocol you’re using:

- **Application Layer:** HTTP, WebSocket, FTP

- **Transport Layer:** QUIC, TCP, UDP

- **Other:** Bonjour service discovery, DNS, Peer-to-peer networking, Wi-Fi

### HTTP

For HTTP, including HTTPS, there is one really good choice: Foundation’s URL Loading System, commonly known as `URLSession`. It supports all the latest features, including Swift concurrency and the HTTP/2 and HTTP/3 protocols.

For more options, see HTTP alternatives.

`URLSession` background sessions allow your app to run an HTTP transfer that continues even if the app stops running. This is most important on iOS, tvOS, and watchOS, where the system suspends your app shortly after the user moves it to the background. To learn more about this feature, see Downloading Files in the Background. Alternative HTTP APIs don’t support this feature.

### WebSocket

For WebSocket you have two choices:

- `URLSession` using URLSessionWebSocketTask

- Network framework using NWConnection (Swift) or nw_connection_t (C-based languages)

Unless you have a specific reason to use `URLSession`, use Network framework for new WebSocket code.

For more options, see WebSocket alternatives.

### FTP

FTP is a very old and dilapidated protocol. FTP is inappropriate to use on the modern internet because it provides *no* security. Because of this, Apple has no supported FTP APIs.

Your best option here is to switch to a newer protocol, like HTTP. It may require some coordination with your server folks, but that will pay off in the long term.

For other options, see FTP alternatives.

### QUIC

Network framework introduced QUIC support in 2021 (see Versions). It supports both QUIC client and QUIC server development.

The QUIC protocol has significant advantages over TCP. If you’re building a custom network protocol, consider using QUIC instead of TCP.

Important

QUIC is a key component of HTTP/3. If your ultimate goal is to support HTTP/3, use `URLSession`. It has direct support for HTTP/3. Network framework’s QUIC support allows you to create custom network protocols running over QUIC.

### TCP

For TCP you have two reasonable options:

- Network framework using NWConnection (Swift) or nw_connection_t (C-based languages)

- BSD Sockets

Network framework is by far the best choice. BSD Sockets is an acceptable choice if you have compatibility constraints, for example:

- When writing cross-platform code

- When using an existing library that’s based on BSD Sockets

For more options, see TCP alternatives. If you decide to use BSD Sockets, read BSD Sockets best practices.

### UDP

For UDP you have two reasonable options:

- Network framework using NWConnection (Swift) or nw_connection_t (C-based languages)

- BSD Sockets

For UDP flows—where you have a stream of unicast datagrams flowing between two peers—Network framework is the best choice. If you use BSD Sockets for this case, you’ll have to do a bunch of extra work.

However, not all UDP communication is that straightforward. UDP also supports multicast, broadcast, and other asymmetric designs. Network framework supports UDP multicast using the NWConnectionGroup class, but that support has limits and, specifically, it does not support UDP broadcast. If you need something that’s not supported by Network framework, use BSD Sockets.

Note

If you’re using UDP to implement a service discovery protocol, consider adopting Bonjour instead. For more details, see Bonjour service discovery.

Regardless of the API you use, if you work with multicast or broadcast UDP on iOS, you must have the multicast networking entitlement. For the details, see com.apple.developer.networking.multicast.

For more options, see UDP alternatives. If you decide to use BSD Sockets, read BSD Sockets best practices.

### Bonjour service discovery

Bonjour is an Apple term for three industry standard technologies: link-local addresses (RFC 3927), multicast DNS (RFC 6762), and DNS-based service discovery (RFC 6763). Use Bonjour to create network features that work well even if there’s no network infrastructure. For example, when you browse for network servers using Finder \> Go \> Connect to Server, you’re using Bonjour.

Bonjour enables three fundamental operations:

- Advertise, to publish a service on the network so that clients can find it by browsing

- Browse, to browse for services on a network so that the user can choose a service

- Connect, to connect to a service chosen by the user

Network framework is your best option for all three of these operations.

If you have specialist needs that aren’t covered by Network framework—for example, you want to resolve a service without connecting to it—use the low-level dnssd API.

On iOS, regardless of what Bonjour API you use, declare your service types in the NSBonjourServices property.

For more options, see Bonjour alternatives.

### Peer-to-peer networking

Peer-to-peer Wi-Fi allows you to communicate with a service on another local device even if that device is not on the same network. Network framework supports peer-to-peer Wi-Fi, but you must opt in to it. To do that, set the includePeerToPeer property (nw_parameters_set_include_peer_to_peer in C) of the parameters object you use to create your connection and listener objects.

Note

The on-the-wire protocol used by peer-to-peer Wi-Fi is not documented for third-party use, so this technique only works between Apple devices.

To communicate between a watchOS app and its companion iOS app, use Watch Connectivity. In many cases, however, it might be better to have your watchOS app operate independently, using `URLSession` to communicate directly with your server.

To connect a tvOS app to a mobile device on the local network, use DeviceDiscoveryUI.

If you’re developing a network-based accessory, consider using Thread. For more background on this, see ThreadNetwork.

For more options, see Peer-to-peer alternatives.

### DNS

In most cases you don’t need to resolve a DNS address manually. Rather, use an API with connect-by-name semantics. For more details, see Connect by name.

To perform advanced DNS operations using the system resolver, use the low-level dnssd API.

To perform DNS queries without using the system resolver—for example, if you’re building a DNS debugging tool—use the `` and `` APIs.

For more options, see DNS alternatives.

### Wi-Fi

iOS supports a number of special-purpose Wi-Fi APIs. For a summary, see TN3111: iOS Wi-Fi API overview.

To scan for and configure Wi-Fi networks on macOS, use Core WLAN.

## Alternative APIs

Many protocols have alternative APIs, ones that are either deprecated or limited to some specific task.

### HTTP alternatives

Apple has two alternative HTTP APIs:

- NSURLConnection is the predecessor to `URLSession`. It’s been redundant since the introduction of `URLSession` in 2013 (see Versions). It was formally deprecated in 2015 (see Versions). Don’t use it for new code. If you have existing `NSURLConnection` code, make a plan to migrate to `URLSession`.

- `CFHTTPStream`, part of the CFNetwork framework, has been deprecated since 2015 (see Versions). Avoid using it in new code. If you have existing `CFHTTPStream` code, make a plan to migrate to something more modern. Typically, that’s `URLSession`.

In some very specific cases, you might find that `URLSession` doesn’t meet your needs. In such cases, you might be able to work around that limitation using `CFHTTPStream`, or perhaps by building a simplistic HTTP client using `CFHTTPMessage` on top of a TCP API. However, building a general-purpose HTTP client is hard. If you need a general-purpose HTTP client and `URLSession` doesn’t work for you, look for a third-party HTTP library. One good option is the AsyncHTTPClient Swift library.

Important

If you need to do some HTTP task that’s not supported by `URLSession`, let us know by filing a suggestion describing your requirements and why `URLSession` doesn’t work for you.

### WebSocket alternatives

Both of the recommended WebSocket APIs were introduced in 2015 (see Versions). If you need to support older OS releases, there are a variety of good quality third-party WebSocket libraries available for Apple platforms.

If you’re currently using a third-party WebSocket library, and your deployment target allows for it, consider moving to Network framework.

### FTP alternatives

Apple has two FTP APIs:

- `URLSession` for FTP downloads, deprecated since 2022 (see Versions)

- `CFFTPStream`, deprecated since 2016 (see Versions)

Don’t write new code using them. If you have existing code, you have two options. The first, and by far the best, is to switch to a newer protocol, like HTTP.

In some circumstances that may not be possible. Perhaps you’re working with an accessory that only supports FTP, and you’re unable to convince the vendor to update its firmware. In that case, you have two options:

- Write your own FTP protocol implementation.

- Adopt a third-party FTP library.

Important

When you evaluate a third-party FTP library, check that it implements FTP directly. If the library uses `CFFTPStream` internally, there’s no point adopting it.

### TCP alternatives

Apple platforms support a variety of alternative TCP APIs:

- `CFSocketStream` was marked as to-be-deprecated in 2021 (see Versions). Apple will not enhance it to support new features. For example, Apple added TLS 1.3 support to Network framework in 2019 (see Versions), but has not added it to `CFSocketStream`.

- The TCP networking support in `NSStream`, most notably getStreamsToHost(withName:port:inputStream:outputStream:), is layered on top of `CFSocketStream` and is on the same deprecation path.

- It’s possible to use FileHandle for networking in conjunction with BSD Sockets. While this is still supported, it’s not recommended for all the same reasons that BSD Sockets is not recommended. See BSD Sockets best practices.

- CFSocket is much like `FileHandle`: It’s possible to use it to run a TCP connection, but it has all the same limitations as BSD Sockets.

- URLSessionStreamTask is much like `URLSessionWebSocketTask`: Unless you have a specific reason to use `URLSession`, use Network framework instead.

- Network Extension in-provider networking includes `NWTCPConnection`. While there are some very limited circumstances where this is still useful, in most cases it’s better to use Network framework. For more details, see In-Provider Networking.

- Foundation has a number of classes, like `NSConnection` and `NSSocketPort`, that *seem* like they might be useful for TCP networking. They are not. These are part of Foundation’s legacy Distributed Objects (DO) system. DO was never a good choice for networking; moreover, it was formally deprecated in 2017 (see Versions).

### UDP alternatives

Network Extension in-provider networking includes `NWUDPSession`. While there are some very limited circumstances where this is still useful, in most cases it’s better to use Network framework. For more details, see In-Provider Networking.

### Bonjour alternatives

There are two older Bonjour APIs:

- NetService

- CFNetService

In 2021 (see Versions) both of these were marked as to-be-deprecated in favor of Network framework.

### Peer-to-peer alternatives

Multipeer Connectivity is a high-level interface to Apple’s peer-to-peer Wi-Fi support. It includes:

- A very opinionated networking model, where every participant in a session is a symmetric peer

- User interface components for advertising and joining a session

Use it when your requirements are aligned with those features. Don’t use it if your program uses a client/server architecture; Network framework works better in that case. For an example, see Building a custom peer-to-peer protocol.

Important

A common misconception is that Multipeer Connectivity is the only way to use peer-to-peer Wi-Fi. That’s not the case. Network framework has opt-in peer-to-peer Wi-Fi support. For the details, see Peer-to-Peer networking.

Foundation also has peer-to-peer Wi-Fi support:

- When advertising a service using `NSNetService`, set the includesPeerToPeer property.

- To accept connections, set the .listenForConnections flag and implement the netService(_:didAcceptConnectionWith:outputStream:) delegate callback.

- When browsing for services using `NSNetServiceBrowser`, set the includesPeerToPeer property.

- After discovering a service with a peer-to-peer enabled browser, connect to that service using getInputStream(_:outputStream:).

These APIs were marked as to-be-deprecated in 2021 (see Versions). If you have existing code that uses them, make a plan to migrate to Network framework.

The dnssd API supports peer-to-peer Wi-Fi but with an important caveat: If you advertise a service on peer-to-peer Wi-Fi using dnssd, the service’s listener must be run by a peer-to-peer aware API, like `NWListener` or `NSNetService`. Given that those APIs already have a facility to opt in to peer-to-peer Wi-Fi, there’s very little point using dnssd for this.

### DNS alternatives

`NSHost` supports synchronous DNS name-to-address and address-to-name translation. It was only ever supported on macOS.

`CFHost` supports DNS name-to-address and address-to-name translation, both synchronously and asynchronously.

Both of these APIs were marked as to-be-deprecated in 2021 (see Versions). If you have existing code that uses them, make a plan to migrate to a preferred API. In many cases that means switching to a connect-by-name API. See Connect by name. For other cases, see DNS.

## Best practices

Apple’s preferred networking APIs, including URLSession and Network framework, implement various best practices by default. If you choose to use an alternative API, you take on the responsibility of implementing these best practices yourself. This section addresses some of the more common issues.

### Connect by name

Traditionally, you connect to a TCP service using two steps:

1.  Resolve the DNS name to a set of IPv4 and IPv6 addresses.

2.  Connect to one of those addresses.

This two-step approach is an anti-pattern on Apple platforms for two reasons:

- It doesn’t support on-demand connections, such as VPN On Demand.

- It’s hard to implement the second step correctly. The industry standard for this is called the *Happy Eyeballs* algorithm (RFC 8305). It’s a non-trivial amount of work.

Apple’s preferred networking APIs support connect-by-name semantics, where you pass the API a DNS name and it takes care of all the details. If you can use a connect-by-name API, do that. If you can’t—and the prime offender here is BSD Sockets—you’ll have to implement Happy Eyeballs yourself.

Sadly, even with all of that extra code, your program will still be incompatible with VPN On Demand.

### BSD Sockets best practices

BSD Sockets has a number of limitations. Your life will be easier if you use Network framework rather than BSD Sockets. If that’s not possible—say you’re working on a cross-platform codebase that mandates the use of sockets—apply the following best practices:

- Implement your own connect-by-name semantics. If you don’t do this, your program might fail to connect, or connect very slowly, in adverse network conditions. For more details, see Connect by name.

- Write code that supports both IPv4 and IPv6. Test that code on an IPv6-only network. See Test for IPv6 DNS64/NAT64 Compatibility Regularly.

- Use the system DNS resolver. For more on this, see DNS best practices.

- BSD Sockets does not support TLS directly. If you want secure connections, and really you should, add your own TLS implementation. For more on this, see TLS best practices.

- Once you’ve established a connection, use SCNetworkReachabilityCreateWithAddressPair(_:_:_:) to monitor its viability. Without this, your program won’t notice that a connection is stuck due to a TCP/IP stack reconfiguration.

Important

If you don’t follow these best practices your networking code will fail in some specific network environments. Such environments are hard to replicate at your workplace, so you might only notice the problem when your program fails after it’s been deployed.

If your primary reason for using BSD Sockets is cross-platform support, consider using a network abstraction layer that adapts to the target platform. One such option is SwiftNIO Transport Services, which makes it straightforward to use Network framework on Apple platforms and BSD Sockets elsewhere.

Apple’s BSD Sockets implementation is documented in the man pages. If you’re unfamiliar with that term, see Reading UNIX Manual Pages. Man pages are notoriously succinct. If you’re getting started with BSD Sockets, take advantage of the wide range of non-Apple resources out there. A classic work in the field is the book *UNIX Network Programming* by Stevens et al.

One traditional challenge with BSD Sockets is how best to handle nonblocking sockets. For cross-platform code you have all the usual options (`select`, `poll`, `kqueue`). For Apple-specific code you have one more: a Dispatch read source. Use this to integrate a nonblocking socket into existing code that uses Dispatch queues. For more details, see Dispatch Source.

Note

If you’re using CFSocket to handle a nonblocking socket, consider switching to a Dispatch read source.

### DNS best practices

Use the system DNS resolver. Implementing your own DNS resolver is extra work, wastes resources, and causes problems in specific network environments.

If you’re using BSD Sockets, use the `getaddrinfo` and `getnameinfo` APIs. BSD Sockets has a range of legacy DNS APIs, like `gethostbyname`, that embody known anti-patterns. For example, `gethostbyname` doesn’t support IPv6 and relies on thread-local storage.

Also use `getaddrinfo` and `getnameinfo` to convert between strings and IP addresses. Again, the legacy APIs for this have various problems. For example, `inet_addr` doesn’t support IPv6 and relies on thread-local storage. When converting an IP address to a string, pass `AI_NUMERICHOST` and `AI_NUMERICSERV` to `getaddrinfo` to ensure that it doesn’t generate any network traffic. Likewise, when going the other way, pass `NI_NUMERICHOST` and `NI_NUMERICSERV` to `getnameinfo`.

If you’re using BSD Sockets and want to resolve a DNS address asynchronously, use DNSServiceGetAddrInfo(_:_:_:_:_:_:_:).

### TLS best practices

Apple’s preferred networking APIs, including URLSession and Network framework, use a built-in, modern TLS stack. That’s not available if you use BSD Sockets. To use TLS in that case, add your own TLS implementation.

Make sure your TLS implementation uses Apple’s trust evaluation infrastructure. If you implement your own trust evaluation, it won’t match that of the built-in apps, like Safari and Mail. For more about Apple’s trust evaluation APIs, see Trust.

Don’t use Secure Transport for your TLS implementation. It’s been deprecated since 2019 (see Versions) and doesn’t support TLS 1.3. If you have existing code that uses Secure Transport, make a plan to migrate off it.

## Versions

Networking is fundamental to all Apple platforms. When Apple introduces a new networking API, or adds new support to an existing API, it typically does so on all platforms. Likewise when Apple deprecates an API. When this technote covers such topics, it references the year of the OS release. The following table maps years to OS version numbers:

| Year | macOS | iOS, tvOS | watchOS |
|------|-------|-----------|---------|
| 2013 | 10.9  | 7         | \-      |
| 2014 | 10.10 | 8         | 1       |
| 2015 | 10.11 | 9         | 2       |
| 2016 | 10.12 | 10        | 3       |
| 2017 | 10.13 | 11        | 4       |
| 2018 | 10.14 | 12        | 5       |
| 2019 | 10.15 | 13        | 6       |
| 2020 | 11    | 14        | 7       |
| 2021 | 12    | 15        | 8       |
| 2022 | 13    | 16        | 9       |

## Revision History

- **2023-09-19** Added information about `CFSocket`.

- **2023-06-06** First published.

## See Also

### Latest

TN3182: Adding privacy tracking keys to your privacy manifest

Declare the tracking domains you use in your app or third-party SDK in a privacy manifest.

TN3183: Adding required reason API entries to your privacy manifest

Declare the APIs that can potentially fingerprint devices in your app or third-party SDK in a privacy manifest.

TN3184: Adding data collection details to your privacy manifest

Declare the data your app or third-party SDK collects in a privacy manifest.

TN3181: Debugging an invalid privacy manifest

Identify common configurations that cause unsuccessful privacy manifest validation with the App Store.

TN3180: Reverting to App Store Server Notifications V1

Migrate from version 2 to version 1 of App Store Server Notifications using the Modify an App endpoint.

TN3179: Understanding local network privacy

Learn how local network privacy affects your software.

TN3178: Checking for and resolving build UUID problems

Ensure that every Mach-O image has a UUID, and that every distinct Mach-O image has its own unique UUID.

TN3177: Understanding alternate audio track groups in movie files

Learn how alternate groups collect audio tracks, and how to choose which audio track to use in your app.

TN3111: iOS Wi-Fi API overview

Explore the various Wi-Fi APIs available on iOS and their expected use cases.

TN3176: Troubleshooting Apple Pay payment processing issues

Diagnose errors that occur when processing Apple Pay payments, identify common causes, and explore potential solutions.

TN3175: Diagnosing issues with displaying the Apple Pay button on your website

Diagnose common errors received while displaying the Apple Pay button on your website by identifying the underlying causes, and explore potential solutions.

TN3174: Diagnosing issues with the Apple Pay payment sheet on your website

Diagnose errors received while presenting the Apple Pay payment sheet on your website by identifying the underlying causes of common errors and explore their potential solutions.

TN3173: Troubleshooting issues with your Apple Pay merchant identifier configuration

Diagnose errors due to invalid Apple Pay merchant identifier configurations by identifying the underlying causes of common errors and explore their potential solutions.

TN3168: Making your App Clip available in the App Store

Learn how to configure your App Clip to prevent it from being unavailable in the App Store.

TN3124: Debugging coordinate space issues

Learn techniques to help debug any coordinate space issue.

