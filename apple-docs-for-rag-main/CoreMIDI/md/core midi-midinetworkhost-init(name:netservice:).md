

- Core MIDI
- MIDINetworkHost
-  init(name:netService:) 

Initializer

# init(name:netService:)

Creates a host with the specified name and net service.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
convenience init(
    name: String,
    netService: NetService
)
```

## Parameters 

`name`  

The host name.

`netService`  

The net service.

## See Also

### Creating Network Hosts

convenience init(name: String, address: String, port: Int)

Creates a host with the specified name, adress, and port.

convenience init(name: String, netServiceName: String, netServiceDomain: String)

Creates a host with the specified name, net service name, and domain.

let MIDINetworkBonjourServiceType: String

The Bonjour service type.

