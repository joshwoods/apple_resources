

- Device Management
-  8021XFirstEthernet 

Device Management Profile

# 8021XFirstEthernet

The payload you use to configure the first wired Ethernet interface.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
WiFi.EAPClientConfiguration 8021XFirstEthernet
```

## Discussion

Specify `com.apple.firstethernet.managed` as the payload type.

This payload’s contents contain these profile-specific keys:

Interface (String)  
This payload uses the value `FirstEthernet`.

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
            FirstEthernet
            Password
            password
            ProxyType
            None
            SetupModes

                System

            PayloadIdentifier
            com.example.my8021Xfirstepayload
            PayloadType
            com.apple.firstethernet.managed
            PayloadUUID
            b0062f3a-8045-410b-82d2-a926a3957f02
            PayloadVersion
            1

    PayloadDisplayName
    802.1x First Ethernet
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    72d32ec9-864e-4f8a-8645-25539172e921
    PayloadVersion
    1

```

## See Also

### Ethernet

object 8021XGlobalEthernet

The payload you use to configure the default fallback global Ethernet interface.

type 8021XFirstActiveEthernet

The payload you use to configure the first wired, active Ethernet interface.

type 8021XSecondActiveEthernet

The payload you use to configure the second wired, active Ethernet interface.

type 8021XSecondEthernet

The payload you use to configure the second wired Ethernet interface.

type 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

type 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

