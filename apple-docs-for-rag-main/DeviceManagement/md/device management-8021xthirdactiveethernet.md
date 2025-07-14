

- Device Management
-  8021XThirdActiveEthernet 

Device Management Profile

# 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
WiFi.EAPClientConfiguration 8021XThirdActiveEthernet
```

## Discussion

Specify `com.apple.thirdactiveethernet.managed` as the payload type.

This payload’s contents contain these profile-specific keys:

Interface (String)  
This payload uses the value `ThirdActiveEthernet`.

EAPClientConfiguration (WiFi.EAPClientConfiguration)  
The dictionary that defines the enterprise profile for the network.

SetupModes (String)  
The type of connection mode, which is either “System” or “Loginwindow.” “System” is the default.

Payloads with `active` in their name apply to Ethernet interfaces that are working at the time of profile installation. If there’s no active Ethernet interface working, this payload configures the interface with the highest service-order priority.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | macOS |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | \-    |

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
            ThirdActiveEthernet
            Password
            password
            ProxyType
            None
            SetupModes

                System

            PayloadIdentifier
            com.example.my8021xthirdaepayload
            PayloadType
            com.apple.thirdactiveethernet.managed
            PayloadUUID
            a001a09a-d40d-4535-83ea-b21c409a5949
            PayloadVersion
            1

    PayloadDisplayName
    802.1x Third Active Ethernet
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    77d92cd3-d303-4e2e-8c67-b6e67b30ba2c
    PayloadVersion
    1

```

## See Also

### Ethernet

object 8021XGlobalEthernet

The payload you use to configure the default fallback global Ethernet interface.

type 8021XFirstActiveEthernet

The payload you use to configure the first wired, active Ethernet interface.

type 8021XFirstEthernet

The payload you use to configure the first wired Ethernet interface.

type 8021XSecondActiveEthernet

The payload you use to configure the second wired, active Ethernet interface.

type 8021XSecondEthernet

The payload you use to configure the second wired Ethernet interface.

type 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

