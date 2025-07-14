

- Network Extension
- NWHostEndpoint
-  init(hostname:port:) Deprecated

Initializer

# init(hostname:port:)

Create a host endpoint with a hostname and port.

iOS 9.0–18.0DeprecatediPadOS 9.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.11–15.0DeprecatedtvOS 17.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
convenience init(
    hostname: String,
    port: String
)
```

Deprecated

Use the nw_endpoint_create_host(_:_:) function from the Network framework instead.

## Parameters 

`hostname`  

A string representation of the hostname or address, such as `www.example.com` or `10.0.0.1`.

`port`  

A string containing the port on the host, such as `80`.

## Discussion

If the hostname is a domain name, such as `www.example.com`, starting a connection to the host endpoint causes the hostname to be resolved to an address during the connection process. If the hostname is an IPv4 or IPv6 address, such as `10.0.0.1` or `fe80::1`, starting a connection to the host endpoint will cause the address to be used directly.

