

- Device Management
-  8021XGlobalEthernet 

Device Management Profile

# 8021XGlobalEthernet

The payload you use to configure the default fallback global Ethernet interface.

iOS 17.0+iPadOS 17.0+macOS 10.13+tvOS 17.0+Device Assignment ServicesVPP License Management

``` source
object 8021XGlobalEthernet
```

## Properties

`ANY`

`any`

Keys relevant to 802.1X configuration. User enrollment payloads don’t support the various proxy keys, including `ProxyType`, `ProxyServer`, `ProxyServerPort`, `ProxyUsername`, `ProxyPassword`, `ProxyPACURL` and `ProxyPACFallbackAllowed`.

## Discussion

Specify `com.apple.globalethernet.managed` as the payload type.

This payload’s contents contain these profile-specific keys:

Interface (String)  
This payload uses the value `GlobalEthernet`.

EAPClientConfiguration (WiFi.EAPClientConfiguration)  
The dictionary that defines the enterprise profile for the network.

SetupModes (String)  
The type of connection mode, which is either “System” or “Loginwindow.” “System” is the default.

### Profile Availability

|                            |                    |
|----------------------------|--------------------|
| Device Channel             | macOS, Shared iPad |
| User Channel               | macOS, Shared iPad |
| Allow Manual Install       | iOS, macOS, tvOS   |
| Requires Supervision       | \-                 |
| Requires User Approved MDM | \-                 |
| Allowed in User Enrollment | iOS, macOS, tvOS   |
| Allow Multiple Payloads    | \-                 |

### Profile Example

```

    PayloadContent

            AuthenticationMethod

            AutoJoin

            CaptiveBypass

            EAPClientConfiguration

                AcceptEAPTypes

                    25

                UserName
                user
                UserPassword
                password

            EncryptionType
            WPA2
            HIDDEN_NETWORK

            Interface
            GlobalEthernet
            Password
            password
            ProxyType
            None
            SetupModes

                System

            PayloadIdentifier
            com.example.myglobalethpayload
            PayloadType
            com.apple.globalethernet.managed
            PayloadUUID
            f3d469f1-d7cc-45c5-ac2d-024195a6454b
            PayloadVersion
            1

    PayloadDisplayName
    802.1x Global Ethernet
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    9a0d652e-1ace-450c-9449-7bcc5d1d62c4
    PayloadVersion
    1

```

## See Also

### Ethernet

type 8021XFirstActiveEthernet

The payload you use to configure the first wired, active Ethernet interface.

type 8021XFirstEthernet

The payload you use to configure the first wired Ethernet interface.

type 8021XSecondActiveEthernet

The payload you use to configure the second wired, active Ethernet interface.

type 8021XSecondEthernet

The payload you use to configure the second wired Ethernet interface.

type 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

type 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

