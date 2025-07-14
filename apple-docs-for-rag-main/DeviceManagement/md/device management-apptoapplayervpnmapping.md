

- Device Management
-  AppToAppLayerVPNMapping 

Device Management Profile

# AppToAppLayerVPNMapping

The payload you use to configure per-app VPN settings.

macOS 10.9+Device Assignment ServicesVPP License Management

``` source
object AppToAppLayerVPNMapping
```

## Properties

`AppLayerVPNMapping`

`[`AppToAppLayerVPNMapping.AppLayerVPNMappingItem`]`

 (Required) 

The array of VPN mapping dictionaries.

## Discussion

Specify `com.apple.vpn.managed.appmapping` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | \-    |
| Allow Multiple Payloads    | \-    |

### Profile Example

```

    PayloadContent

            IPSec

                RemoteAddress
                10.0.1.42
                XAuthName
                username
                OnDemandEnabled
                0
                XAuthPassword
                password
                AuthenticationMethod
                None
                LocalIdentifier
                outside-psk-full
                PromptForVPNPIN

            IPv4

                OverridePrimary
                0

            Proxies

            UserDefinedName
            outside-asa-ipsec-full
            VPN

                RemoteAddress
                10.0.1.42
                DisconnectOnIdle
                0
                AuthName
                username
                AuthPassword

                AuthenticationMethod
                password

            VPNType
            VPN
            VendorConfig

                Group

            VPNSubType
            com.cisco.anyconnect.applevpn.plugin
            VPNUUID
            beb2dc33-280d-48ce-a2f6-9e164cccc18a
            OnDemandMatchAppEnabled

            PayloadIdentifier
            com.example.myvpnmanagedapplayerpayload
            PayloadType
            com.apple.vpn.managed.applayer
            PayloadUUID
            6A0806DD-6BA7-41A0-A612-FDE7D4B6959D
            PayloadVersion
            1

            AppLayerVPNMapping

                    VPNUUID
                    beb2dc33-280d-48ce-a2f6-9e164cccc18a
                    Identifier
                    come.example.firefox
                    DesignatedRequirement
                    anchor apple generic and certificate leaf[field.9.8.765.432109.876.5.4.3] /* exists */ or anchor apple generic and certificate 1[field.9.8.765.432109.876.5.4.3] /* exists */ and certificate leaf[field.9.8.765.432109.876.5.4.3] /* exists */ and certificate leaf[subject.OU] = &quot;ABCDE12345&quot;
                    SigningIdentifier
                    ABCDE12345

            PayloadIdentifier
            com.example.myapplayvpnmappingpayload
            PayloadType
            com.apple.vpn.managed.appmapping
            PayloadUUID
            3B9E6DC0-1644-4CD1-908B-C970F7213F2D
            PayloadVersion
            1

    PayloadDisplayName
    App to App Layer VPN Mapping
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    6E65044E-AEDC-4671-ACF4-80042CD53B2D
    PayloadVersion
    1

```

## Topics

### Objects

object AppToAppLayerVPNMapping.AppLayerVPNMappingItem

A dictionary defining a per-app VPN relationship.

## See Also

### VPN

object AppLayerVPN

The payload you use to configure add-on VPN software.

object VPN

The payload you use to configure a VPN.

