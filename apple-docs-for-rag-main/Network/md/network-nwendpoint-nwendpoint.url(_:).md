

- Network
- NWEndpoint
-  NWEndpoint.url(\_:) 

Case

# NWEndpoint.url(\_:)

An endpoint represented as a URL, with host and port values inferred from the URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
case url(URL)
```

## See Also

### Endpoint Types

case hostPort(host: NWEndpoint.Host, port: NWEndpoint.Port)

An endpoint represented as a host and port, with the host including both names and addresses.

case service(name: String, type: String, domain: String, interface: NWInterface?)

An endpoint represented as a Bonjour service.

case unix(path: String)

An endpoint represented as a UNIX domain path.

