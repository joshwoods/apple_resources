

- Device Management
-  8021XSecondActiveEthernet 

Device Management Profile

# 8021XSecondActiveEthernet

The payload you use to configure the second wired, active Ethernet interface.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
WiFi.EAPClientConfiguration 8021XSecondActiveEthernet
```

## Discussion

Specify `com.apple.secondactiveethernet.managed` as the payload type.

This payload’s contents contain these profile-specific keys:

Interface (String)  
This payload uses the value `SecondActiveEthernet`.

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
            SecondActiveEthernet
            Password
            password
            ProxyType
            None
            SetupModes

                System

            PayloadIdentifier
            com.example.my8021Xsecaepayload
            PayloadType
            com.apple.secondactiveethernet.managed
            PayloadUUID
            38791a67-90ca-40e5-bddd-fc3dc85a447e
            PayloadVersion
            1

    PayloadDisplayName
    802.1x Second Active Ethernet
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    50939eda-ff93-4e0c-907b-159d8d5c1a1a
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

type 8021XSecondEthernet

The payload you use to configure the second wired Ethernet interface.

type 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

type 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

