

- Device Management
-  8021XThirdEthernet 

Device Management Profile

# 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
WiFi.EAPClientConfiguration 8021XThirdEthernet
```

## Discussion

Specify `com.apple.thirdethernet.managed` as the payload type.

This payload’s contents contain these profile-specific keys:

Interface (String)  
This payload uses the value `ThirdEthernet`.

EAPClientConfiguration (WiFi.EAPClientConfiguration)  
The dictionary that defines the enterprise profile for the network.

SetupModes (String)  
The type of connection mode, which is either “System” or “Loginwindow.” “System” is the default.

This payload applies to Ethernet interfaces according to service order, regardless of whether the interface is working.

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
            ThirdEthernet
            Password
            password
            ProxyType
            None
            SetupModes

                System

            PayloadIdentifier
            com.example.my8021Xthirdepayload
            PayloadType
            com.apple.thirdethernet.managed
            PayloadUUID
            bffa7d6f-fd20-45c0-a5f4-6fc5bd37c23f
            PayloadVersion
            1

    PayloadDisplayName
    802.1x Third Ethernet
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    05c2aeaa-954e-4704-87a6-e4cff93cfd25
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

type 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

