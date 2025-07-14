

- Network Extension
- NENetworkRule
-  init(destinationHost:protocol:) Deprecated

Initializer

# init(destinationHost:protocol:)

Creates a rule that matches network traffic destined for a host within a specific DNS domain.

macOS 10.15–15.0Deprecated

``` source
init(
    destinationHost hostEndpoint: NWHostEndpoint,
    protocol: NENetworkRule.Protocol
)
```

## Parameters 

`hostEndpoint`  

An endpoint instance that contains the port and hostname or domain that the rule matches. This endpoint must contain a hostname, not an address.

`protocol`  

The protocol that the rule matches.

## Discussion

If the port string of `destinationHost` is `0` or is the empty string, then the rule matches traffic on any port destined for the given hostname or domain.

If the hostname string of `destinationHost` consists of a single label, then the rule matches traffic destined to the specific host with that single label as its name.

If the hostname string of `destinationHost` consists of two or more labels, then the rule matches traffic destined to hosts within the domain specified by the hostname string.

### Examples

The following example makes a rule that matches all TCP and UDP traffic to a host named `com` in Swift.

```
let endpoint = NWHostEndpoint(hostname: "com", port: "0")
let rule = NENetworkRule(destinationHost: endpoint, protocol: .any)
```

Here’s the same example in ObjectiveC.

```
NWHostEndpoint *endpoint = [NWHostEndpoint endpointWithHostname:@"com"
                                                           port:@"0"];

NENetworkRule *rule = [[NENetworkRule alloc] initWithDestinationHost:endpoint
                                                            protocol:NENetworkRuleProtocolAny];
```

The next example matches all TCP and UDP traffic to hosts in the `example.com` DNS domain, including all DNS queries for names in the `example.com` DNS domain.

```
let endpoint = NWHostEndpoint(hostname: "example.com", port: "0")
let rule = NENetworkRule(destinationHost: endpoint, protocol: .any)
```

Here’s the same example in ObjectiveC.

```
NWHostEndpoint *endpoint = [NWHostEndpoint endpointWithHostname:@"example.com"
                                                           port:@"0"];

NENetworkRule *rule = [[NENetworkRule alloc] initWithDestinationHost:endpoint
                                                            protocol:NENetworkRuleProtocolAny];
```

The next example makes a rule that matches all DNS queries and responses for hosts in the `example.com` domain.

```
let endpoint = NWHostEndpoint(hostname: "example.com", port: "53")
let rule = NENetworkRule(destinationHost: endpoint, protocol: .any)
```

Here’s the same example in ObjectiveC.

```
NWHostEndpoint *endpoint = [NWHostEndpoint endpointWithHostname:@"example.com"
                                                           port:@"53"];

NENetworkRule *rule = [[NENetworkRule alloc] initWithDestinationHost:endpoint
                                                            protocol:NENetworkRuleProtocolAny];
```

The last example makes a rule that matches all TCP port 443 traffic to hosts in the `example.com` domain.

```
let endpoint = NWHostEndpoint(hostname: "example.com", port: "443")
let rule = NENetworkRule(destinationHost: endpoint, protocol: .TCP)
```

Here’s the same example in ObjectiveC.

```
NWHostEndpoint *endpoint = [NWHostEndpoint endpointWithHostname:@"example.com"
                                                           port:@"443"];

NENetworkRule *rule = [[NENetworkRule alloc] initWithDestinationHost:endpoint
                                                            protocol:NENetworkRuleProtocolTCP];
```

## See Also

### Creating a network rule

init(destinationNetwork: NWHostEndpoint, prefix: Int, protocol: NENetworkRule.Protocol)

Creates a rule that matches network traffic destined for a host within a specific network.

Deprecated

init(remoteNetwork: NWHostEndpoint?, remotePrefix: Int, localNetwork: NWHostEndpoint?, localPrefix: Int, protocol: NENetworkRule.Protocol, direction: NETrafficDirection)

Creates a rule that matches traffic by remote network, local network, protocol, and direction.

Deprecated

