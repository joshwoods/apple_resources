

- Device Management
- WiFi
-  WiFi.QoSMarkingPolicy 

Device Management Profile

# WiFi.QoSMarkingPolicy

A dictionary that defines the quality-of-service settings.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.2+Device Assignment ServicesVPP License Management

``` source
object WiFi.QoSMarkingPolicy
```

## Properties

`QoSMarkingAppleAudioVideoCalls`

`boolean`

If `true`, adds audio and video traffic of built-in audio/video services, such as FaceTime and Wi-Fi Calling, to the allow list for L2 and L3 marking for traffic that goes to the Wi-Fi network.

Default: `true`

`QoSMarkingEnabled`

`boolean`

If `true`, disables L3 marking and only uses L2 marking for traffic that goes to the Wi-Fi network.

If `false`, the system behaves as if Wi-Fi doesn’t have an association with a Cisco QoS fast lane network.

Default: `true`

`QoSMarkingAllowListAppIdentifiers`

`[string]`

An array of app bundle identifiers that defines the allow list for L2 and L3 marking for traffic that goes to the Wi-Fi network. If the array isn’t present, but the `QoSMarkingPolicy` key is present — even empty — no apps can use L2 and L3 marking.

`QoSMarkingWhitelistedAppIdentifiers`

`[string]`

Deprecated 

Use `QoSMarkingAllowListAppIdentifiers` instead.

## Discussion

When this dictionary isn’t present for a Wi-Fi network, all apps can use L2 and L3 marking when the Wi-Fi network supports Cisco QoS fast lane. When present in the Wi-Fi payload, the `QoSMarkingPolicy` dictionary needs to contain the list of allowed apps to benefit from L2 and L3 marking.

## See Also

### Objects

object WiFi.EAPClientConfiguration

A dictionary that configures an enterprise network.

