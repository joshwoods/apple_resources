

- Core MIDI
- MIDINetworkHost
-  init(name:netServiceName:netServiceDomain:) 

Initializer

# init(name:netServiceName:netServiceDomain:)

Creates a host with the specified name, net service name, and domain.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
convenience init(
    name: String,
    netServiceName: String,
    netServiceDomain: String
)
```

## Parameters 

`name`  

The host name.

`netServiceName`  

The net service name.

`netServiceDomain`  

The net service domain.

## See Also

### Creating Network Hosts

convenience init(name: String, address: String, port: Int)

Creates a host with the specified name, adress, and port.

convenience init(name: String, netService: NetService)

Creates a host with the specified name and net service.

let MIDINetworkBonjourServiceType: String

The Bonjour service type.

