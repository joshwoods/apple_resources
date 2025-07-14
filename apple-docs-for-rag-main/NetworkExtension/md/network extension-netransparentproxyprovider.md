

- Network Extension
-  NETransparentProxyProvider 

Class

# NETransparentProxyProvider

An object that implements the client side of a custom transparent network proxy solution.

macOS 11.0+

``` source
class NETransparentProxyProvider
```

## Mentioned in 

Handling Flow Copying

## Overview

The NETransparentProxyProvider class has the following behavior differences from its superclass NEAppProxyProvider:

- Returning `NO` from handleNewFlow(_:) and handleNewUDPFlow(_:initialRemoteEndpoint:) causes the flow to proceed to communicate directly with the flow’s ultimate destination, instead of closing the flow with a “Connection Refused” error.

- This provider ignores NEDNSSettings and NEProxySettings specified within NETransparentProxyNetworkSettings. Flows that match the includedNetworkRules within NETransparentProxyNetworkSettings use the same DNS and proxy settings that other flows on the system currently use.

- Flows that are created using a “connect by name” API (such as Network framework or URLSession) that match the includedNetworkRules don’t bypass DNS resolution.

## Relationships

### Inherits From

- NEAppProxyProvider

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Transparent proxy configuration

class NETransparentProxyManager

An object that configures and controls transparent proxies.

class NETransparentProxyNetworkSettings

A specification of what traffic to route through a transparent proxy.

class NENetworkRule

A rule to match attributes of network traffic.

