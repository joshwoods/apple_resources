

- Network Extension
- NETransparentProxyNetworkSettings
-  includedNetworkRules 

Instance Property

# includedNetworkRules

An array of rules that collectively specify what traffic to route through the transparent proxy.

macOS 10.15+

``` source
var includedNetworkRules: [NENetworkRule]? { get set }
```

## Discussion

The following restrictions apply to each rule in the array:

- If the port string of the endpoint is `0` or is the empty string, then the address of the endpoint must be a non-wildcard address, such as `0.0.0.0` or `::`.

- If the address is a wildcard address (such as `0.0.0.0` or `::)`, then the port string of the endpoint must be non-empty and must not be `0`.

- A port string of `53` is not allowed. Use Destination Domain-based rules to match DNS traffic.

- The matchLocalNetwork property must be `nil`.

- The matchDirection property must be NETrafficDirection.outbound.

## See Also

### Traffic routing rules

var excludedNetworkRules: [NENetworkRule]?

An array of rules that collectively specify what traffic to not route through the transparent proxy.

