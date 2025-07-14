

- Device Management
-  8021XSecondEthernet 

Device Management Profile

# 8021XSecondEthernet

The payload you use to configure the second wired Ethernet interface.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
WiFi.EAPClientConfiguration 8021XSecondEthernet
```

## Discussion

Specify `com.apple.secondethernet.managed` as the payload type.

This payload’s contents contain these profile-specific keys:

Interface (String)  
This payload uses the value `SecondEthernet`.

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
            SecondEthernet
            Password
            password
            ProxyType
            None
            SetupModes

                System

            PayloadIdentifier
            com.example.my8021XsecEpayload
            PayloadType
            com.apple.secondethernet.managed
            PayloadUUID
            37d5702f-299a-4dbe-acd5-d7e8946222f1
            PayloadVersion
            1

    PayloadDisplayName
    802.1x Second Ethernet
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    37490fd4-10c0-4154-8964-9b719e53de31
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

type 8021XThirdActiveEthernet

The payload you use to configure the third wired, active Ethernet interface.

type 8021XThirdEthernet

The payload you use to configure the third wired Ethernet interface.

