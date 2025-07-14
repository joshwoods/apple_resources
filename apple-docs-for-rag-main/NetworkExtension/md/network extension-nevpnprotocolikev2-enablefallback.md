

- Network Extension
- NEVPNProtocolIKEv2
-  enableFallback 

Instance Property

# enableFallback

A property to enable the use of cellular data when Wi-Fi connectivity is poor.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var enableFallback: Bool { get set }
```

## Discussion

Wi-Fi Assist allows connections for foreground apps to switch over to cellular data when Wi-Fi connectivity is poor. When this value is `true`, the device brings up a tunnel over celluar to carry traffic that’s eligible for Wi-Fi Assist and also requires VPN. Enabling fallback requires that the server support multiple tunnels for a single user.

The default value of this property is `false`.

