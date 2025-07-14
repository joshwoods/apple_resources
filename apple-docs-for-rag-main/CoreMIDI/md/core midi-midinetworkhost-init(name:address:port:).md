

- Core MIDI
- MIDINetworkHost
-  init(name:address:port:) 

Initializer

# init(name:address:port:)

Creates a host with the specified name, adress, and port.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
convenience init(
    name: String,
    address: String,
    port: Int
)
```

## Parameters 

`name`  

The host name.

`address`  

The host’s IP address or hostname.

`port`  

The host’s UDP port.

## See Also

### Creating Network Hosts

convenience init(name: String, netService: NetService)

Creates a host with the specified name and net service.

convenience init(name: String, netServiceName: String, netServiceDomain: String)

Creates a host with the specified name, net service name, and domain.

let MIDINetworkBonjourServiceType: String

The Bonjour service type.

