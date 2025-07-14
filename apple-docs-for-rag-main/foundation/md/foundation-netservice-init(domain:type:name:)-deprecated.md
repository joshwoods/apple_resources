

- Foundation
- NetService
-  init(domain:type:name:) Deprecated

Initializer

# init(domain:type:name:)

Returns the receiver, initialized as a network service of a given type and sets the initial host information.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
convenience init(
    domain: String,
    type: String,
    name: String
)
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Parameters 

`domain`  

The domain for the service. To resolve in the default domains, pass in an empty string (`@""`). To limit resolution to the local domain, use `@"local."`.

If you are creating this object to resolve a service whose information your app stored previously, you should set this to the domain in which the service was originally discovered.

You can also use a `NSNetServiceBrowser` object to obtain a list of possible domains in which you can discover and resolve services.

`type`  

The network service type.

`type` must contain both the service type and transport layer information. To ensure that the mDNS responder searches for services, as opposed to hosts, prefix both the service name and transport layer name with an underscore character (”\_”). For example, to search for an HTTP service on TCP, you would use the type string “`_http._tcp.`”. Note that the period character at the end of the string, which indicates that the domain name is an absolute name, is required.

`name`  

The name of the service to resolve.

## Return Value

The receiver, initialized as a network service named `name` of type `type` in the domain `domain`.

## Discussion

This method is the appropriate initializer to use to resolve a service—to publish a service, use init(domain:type:name:port:).

If you know the values for `domain`, `type`, and `name` of the service you wish to connect to, you can create an `NSNetService` object using this initializer and call resolve(withTimeout:) on the result.

You cannot use this initializer to publish a service. This initializer passes an invalid port number to the designated initializer, which prevents the service from being registered. Calling publish() on an `NSNetService` object initialized with this method generates a call to your delegate’s netService(_:didNotPublish:) method with an NetService.ErrorCode.badArgumentError error.

## See Also

### Related Documentation

NSNetServices and CFNetServices Programming Guide

Bonjour Overview

### Creating Network Services

init(domain: String, type: String, name: String, port: Int32)

Initializes the receiver for publishing a network service of type `type` at the socket location specified by `domain`, `name`, and `port`.

Deprecated

