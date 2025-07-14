

- Network Extension
- NENetworkRule
-  init(destinationNetwork:prefix:protocol:) Deprecated

Initializer

# init(destinationNetwork:prefix:protocol:)

Creates a rule that matches network traffic destined for a host within a specific network.

macOS 10.15–15.0Deprecated

``` source
init(
    destinationNetwork networkEndpoint: NWHostEndpoint,
    prefix destinationPrefix: Int,
    protocol: NENetworkRule.Protocol
)
```

## Parameters 

`networkEndpoint`  

An endpoint instance that matches the port and address or network that the rule matches. This endpoint must contain an address, not a hostname.

`destinationPrefix`  

An integer that in combination with the address in the endpoint specifies the destination network that the rule matches.

`protocol`  

The protocol that the rule matches.

## Discussion

If the port string of `networkEndpoint` is `0` or the empty string, the rule matches traffic on any port destined for the given address or network.

## See Also

### Creating a network rule

init(destinationHost: NWHostEndpoint, protocol: NENetworkRule.Protocol)

Creates a rule that matches network traffic destined for a host within a specific DNS domain.

Deprecated

init(remoteNetwork: NWHostEndpoint?, remotePrefix: Int, localNetwork: NWHostEndpoint?, localPrefix: Int, protocol: NENetworkRule.Protocol, direction: NETrafficDirection)

Creates a rule that matches traffic by remote network, local network, protocol, and direction.

Deprecated

