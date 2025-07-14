

- Foundation
- NetService
-  init(domain:type:name:port:) Deprecated

Initializer

# init(domain:type:name:port:)

Initializes the receiver for publishing a network service of type `type` at the socket location specified by `domain`, `name`, and `port`.

iOS 2.0–18.4DeprecatediPadOS 2.0–18.4DeprecatedMac Catalyst 13.1+macOS 10.2–15.4DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–2.4Deprecated

``` source
init(
    domain: String,
    type: String,
    name: String,
    port: Int32
)
```

Deprecated

Use nw_connection_t or nw_listener_t in Network framework instead

## Parameters 

`domain`  

The domain for the service. To use the default registration domains, pass in an empty string (`@""`). To limit registration to the local domain, use `@"local."`.

You can also use a `NSNetServiceBrowser` object to obtain a list of possible domains in which you can publish your service.

`type`  

The network service type.

`type` must contain both the service type and transport layer information. To ensure that the mDNS responder searches for services, as opposed to hosts, prefix both the service name and transport layer name with an underscore character (”\_”). For example, to search for an HTTP service on TCP, you would use the type string “`_http._tcp.`”. Note that the period character at the end of the string, which indicates that the domain name is an absolute name, is required.

`name`  

The name by which the service is identified to the network. The name must be unique. If you pass the empty string (`@""`), the system automatically advertises your service using the computer name as the service name.

`port`  

The port on which the service is published.

If you specify the `NSNetServiceListenForConnections` flag, you may pass zero (`0`), in which case the service automatically allocates an arbitrary (ephemeral) port for your service. When the delegate’s netServiceDidPublish(_:) is called, you can determine the actual port chosen by calling the service object’s NetService method or accessing the corresponding property.

If your app is listening for connections on its own, the value of `port` must be a port number acquired by your application for the service.

## Discussion

You use this method to create a service that you wish to publish on the network. Although you can also use this method to create a service you wish to resolve on the network, it is generally more appropriate to use the init(domain:type:name:) method instead.

When publishing a service, you must provide valid arguments in order to advertise your service correctly. If the host computer has access to multiple registration domains, you must create separate `NSNetService` objects for each domain. If you attempt to publish in a domain for which you do not have registration authority, your request may be denied.

It is acceptable to use an empty string for the `domain` argument when publishing or browsing a service, but do not rely on this for resolution.

This method is the designated initializer.

## See Also

### Creating Network Services

convenience init(domain: String, type: String, name: String)

Returns the receiver, initialized as a network service of a given type and sets the initial host information.

Deprecated

