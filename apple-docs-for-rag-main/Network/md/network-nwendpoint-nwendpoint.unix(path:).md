

- Network
- NWEndpoint
-  NWEndpoint.unix(path:) 

Case

# NWEndpoint.unix(path:)

An endpoint represented as a UNIX domain path.

iOS 12.0+iPadOS 12.0+Mac Catalyst 12.0+macOS 10.14+tvOS 12.0+visionOS 1.0+watchOS 5.0+

``` source
case unix(path: String)
```

## See Also

### Endpoint Types

case hostPort(host: NWEndpoint.Host, port: NWEndpoint.Port)

An endpoint represented as a host and port, with the host including both names and addresses.

case service(name: String, type: String, domain: String, interface: NWInterface?)

An endpoint represented as a Bonjour service.

case url(URL)

An endpoint represented as a URL, with host and port values inferred from the URL.

