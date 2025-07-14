

- Device Management
-  AppLayerVPN 

Device Management Profile

# AppLayerVPN

The payload you use to configure add-on VPN software.

iOS 7.0+iPadOS 7.0+macOS 10.9+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object AppLayerVPN
```

## Properties

`AssociatedDomains`

`[string]`

An array with entries that must each specify a domain that triggers this VPN. The domains must also be part of the `apple-app-site-association` file, as described in Supporting associated domains.

Available in iOS 14 and later, and macOS 11 and later.

`CalendarDomains`

`[string]`

An array with entries that must each specify a domain that triggers this VPN connection in Calendar. Each entry is in the format `www.apple.com`.

This property is deprecated in iOS 13.4 and later; use the `VPNUUID` property of the CalDAV payload instead.

`CellularSliceUUID`

`string`

`ContactsDomains`

`[string]`

An array with entries that must each specify a domain that triggers this VPN connection in Contacts. Each entry is in the format `www.apple.com`.

This property is deprecated in iOS 13.4 and later; use the `VPNUUID` property of the CardDAV payload instead.

`ExcludedDomains`

`[string]`

An array with entries that each specify a domain that doesn’t trigger this VPN for connections to the domain.

Available in iOS 14 and later, and macOS 11 and later.

`MailDomains`

`[string]`

An array with entries that must each specify a domain that triggers this VPN connection in Mail. Each entry is in the format `www.apple.com`.

This property is deprecated in iOS 13.4 and later; use the `VPNUUID` property of the Mail or ExchangeActiveSync payload instead.

`OnDemandMatchAppEnabled`

`boolean`

If `true`, automatically connects the VPN when associated apps for this per-app VPN service initiate network communication. Otherwise, the user must initiate the connection manually before those apps can initiate network communication. If this key isn’t present, the value of the `OnDemandEnabled` key determines the status of per-app VPN On Demand.

`SafariDomains`

`[string]`

An array with entries that must each specify a domain that triggers the VPN connection in Safari. Each entry is in the format `www.apple.com`.

`SMBDomains`

`[string]`

An array of SMB domains that’s accessible through this VPN connection.

Available in iOS 13 and later.

`VPNUUID`

`string`

 (Required) 

A globally unique identifier for this VPN configuration.

## Discussion

Specify `com.apple.vpn.managed.applayer` as the payload type.

This profile defines per-app VPN behavior and only applies to VPN services of type `VPN`, `IPsec`, and `IKEv2`. All the properties of VPN apply to the top level of this profile as well.

### Profile Availability

|                            |                                  |
|----------------------------|----------------------------------|
| Device Channel             | iOS, macOS, Shared iPad, watchOS |
| User Channel               | macOS                            |
| Allow Manual Install       | iOS, macOS                       |
| Requires Supervision       | \-                               |
| Requires User Approved MDM | \-                               |
| Allowed in User Enrollment | iOS, macOS                       |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad, watchOS |

### Profile Example

```

    PayloadContent

            IPSec

                AuthenticationMethod
                SharedSecret
                OnDemandEnabled
                0
                PromptForVPNPIN

            IPv4

                OverridePrimary
                0

            OnDemandMatchAppEnabled

            Proxies

            SafariDomains

                foo.server.com
                *.server.com

            MailDomains

                foo.server.com
                *.server.com

            CalendarDomains

                foo.server.com
                *.server.com

            ContactsDomains

                foo.server.com
                *.server.com

            UserDefinedName
            Per-App VPN
            VPN

                AuthName
                example
                AuthPassword
                password
                AuthenticationMethod
                Certificate
                DisconnectOnIdle
                0
                OnDemandMatchAppEnabled

                PayloadCertificateUUID
                C9BF4927-E819-4521-88DE-2AEB6E1DC3D8
                RemoteAddress
                example.server.com

            VPNSubType
            com.server.server-example.vpnplugin
            VPNType
            VPN
            VPNUUID
            9F658A35-2B0F-4D5E-872D-61A9130FE882
            VendorConfig

                PerAppVpn
                true

            PayloadIdentifier
            com.example.myapplayervpnpayload
            PayloadType
            com.apple.vpn.managed.applayer
            PayloadUUID
            5A015006-D559-4C5C-B197-737CF4DCFA96
            PayloadVersion
            1

            Password
            password
            PayloadCertificateFileName
            identity.p12
            PayloadContent

            MIIL2QIBAzCCC58GCSqGSIb3DQEHAaCCC5AEgguMMIILiDCCBj8GC
            SqGSIb3DQEHBqCCBjAwggYsAgEAMIIGJQYJKoZIhvcNAQcBMBwGCi
            qGSIb3DQEMAQYwDgQIqckvWPHWFRUCAggAgIIF+N4kXpz9g4BBBmU
            T/e+KS5OjAlhPyjtLfXvoKVo0G2MOF4cVrMXr3inoOUc+dOTYEN8y
            7Rt2ls3XzDZCHXikDYFGg8fz7sDgNMJGwsZFdkCqxo0OJcDdJY0e3
            GQZr6MfJlkADFBrJW8rTV2TPiClxUatTjEQBRUlEU0Z6x83f1LzoX
            Xkkn5PFsd002Bjg2eVwe4bA9i2EbFbA2XVDXJ0AOnegV0GOXGJRfM
            4UWQZdR5mnLICTOzLAFi+k+MfkhBG3tTyiisRcSpDhxCWMIIVCjsR
            6TfDFt0PDi4OfmVqPyeRro2Kf8DjE6iZmc2rdin3d3YLOJAkixK/6
            gTMeCBXqv1IMDbIlOzOtM4dNopxZttzmuDg+vUWiworJVBnHfYMT0
            Vtimxv2ER7CAGNWD4pxhetR1iiBnaLQI1lU4DfcPpPxvL9uUx9PDX
            AqAN6uAXoE4Sc0z5Dym73j6T6tb8mNB0Pf2TSxrm2af0bMTTPqEM2
            6i0fqCGhLeU5eB2fq9ED5X6+JjB15Kns4bNVvetS+5HOC59UGBFSS
            9i3vj4SzLqIJ4zFbjltkTl/uWDr4BA3kydIbkD/RNqKlvGEjV3e59
            Y87H4LlN/xwAsM86ht8juR1IhzT6+fj4i2qXdrHRAWTovB6OtPMML
            aAgiRgZqwxnx8UXEG3q6RkMqbhph7O4j3HNgKAW+Z72J/b39ZS0Yv
            ghIfGFsHsrypD4BNqvHaYxJhT3ORscW+M05oQ0vn+hBMs5mPq3mJu
            3Lj2j8xA42Q+XAgZM8w+eCwgYx2AxtOYJuC+mOYTWpb1E7m5Kwx6m
            gANXVurmhEL0KbzzgAg/FMW8EkI9+rZNXpo0wjxCsqSA8NFsAuCHl
            gwJ+A5ifE19gOQqmZ6c4xtHRtxBQ/MO977UKJ8+gV/o/r+DVi5yQ/
            /4CSZkMgdb+kzoWVB/5wzOZrJKqCQJ/+3P0KEk3utamMy8Nq0ubyB
            7r5f6pGcIqQ/gyYqLVFszTYKgwqea22jydboJRXW6fiDXFvI42K3f
            9lQUw7BfwpKaCWo2/bEzYpAz0/EfVKnpQoyfMnnbE/ev8U2VLuiZ5
            1DnLtsK6hS+rxQiH9yx7K+IQgGuj5ARuyQnwWgKrK6rna3b1GP8Fp
            pVH/E+XR4k9q7aY8lyyDaz6kZ+78SveVNtbDE8ClhyVmqVWC67B7A
            G7jq/61ovb1auN2nuY9QyTUKrEtVPmfoZmdE8rn7qkZUm/sQAQLB8
            E4bA1w7dlC6ENFKdHLsXNmow+nUuf+gumiD7T32pDtknVl4guQzbP
            BXzTS3J6UyvkSA+TXGpzpbV47BFOeAgQMD1BX06vlIqqLkkaKu5hd
            LdajmGKbZaL2RHgMsGIE0eRRN9725GNIH0PtytkqieuOdfft2D8Ug
            CFtY/KJM9GystQDV6NggbgcHIFsLct8m+QqJRs3UlBKtqCs1pbySS
            8gdHERyFG/zC5T9yft/tLva0b/YDetq/YzwcZqbfcde/LimuQYe9z
            RtQqVlYjpZctCJnIleIn1QtLNuf0GVVrFkHGz7zWhxU1VB8C0+jsB
            Mz2BP9DZar3Gx4GVyizAf6i9DvyxlY0qjIo2cSAa9XvfVqrtCCPc5
            mu8c+oMlurUljmvcVKOsNsAPW6iB5o22mPFjr3quq1oNgBpmZ2Z7d
            VmOEQww99Bi7FyHCe2Ti5IDXSzBklfeiYNyCgZnEjLbzEXMPK0sN2
            oFHwcdU6OWKfz5MjS4aMm7sUOULUAuP8xy7VArlyb14NVIzhJc5fu
            RYc+vH+K+wHtpcQeNqdBftVd5SllVEgJTKqfSxZbPEC6u0skczudD
            tCR4zHSvYbR1gvVAcpQ+XGBgNVqUCwwM+ctroWpKmYJ3YrwXtGf+T
            KWV99IJLso7MtKBKUFQWXNOQBRgMFQuJ4i3hztaupTEQVuka3qhco
            cak3R242G3P1prlvQNmi6HI3t4jFND+z5DzrsgW11fc/pOgEM6UpB
            Al6WZrSKN+5rJEmGq8tB+GHQ0cELhaNlDgBtqkvcisdf/49VkU6aH
            qJWafQ3HCkwggVBBgkqhkiG9w0BBwGgggUyBIIFLjCCBSowggUmBg
            sqhkiG9w0BDAoBAqCCBO4wggTqMBwGCiqGSIb3DQEMAQMwDgQIrOA
            9tf9ADYICAggABIIEyBZLrSiXbZV1TOqk+2KsrCLj915uIgLakWDP
            YE/f+Puxok/RW/ohdOEV2555WQxR4ip1edvCzKYGYomGLDqimo/c8
            /I0WEjlY7aOgxTz1Vd5MtFFYxRMlSpB+v9/hoR63VwH8VD9gHL3Xy
            8Dg/L0QsdUZ6UTjKD9Apl6L7FgmTczoalM1NBtuy4mMYtkzznZMmD
            mgRsONa/nLB8XcCIoIycHA/qDtDDquNplPsFsoXqvUHsWhidP5jW0
            2fg3WdT9TDPWiJ8qRhvii0LlNAGhjreH5/tClKiTj4ez+o8vmEn0O
            s37jgtzutJYN2h5w2CnsgxGV6Ks2lxkowFx0WL3PHELIN7yWp9z9U
            yY/OItkVLuJNxqk4+LkqIrL8M1aunp+c8CV1oT2sjg7uPQjm6ppoX
            UmhpmY9UBBNhXVeN+ww6mAOCnz9XhwBW9vMTMf3vBjCl68ce4vTCX
            qX7O8DHcPNQ1qhVl/3OlUnJQkqyuwBmd7PCDJuPcC1uNEnfQ9QvB1
            AQFzXeJkW3R0oQDM3uVLKcNN32XID0pD/Dq3DY2hA2XW8nP4Ihf4M
            3eirDu/s9CfmEJ0tDSlEBOYmwyFvsQqzFTtQ6I1yF7CzMCxmBHgmM
            iq5j5zgwIGylWr2vgLT5zP9QFULxoR/CqiQxjXnOtrEjAR2EH4IpD
            bd1nB+WXJdOLBQwWK9eNU1zLAiLP5wAHFVD1wJ4ULxxparWgyzPlM
            pIjsVHgsosrOjZKCGHTiza5VE7Ww+0KeWDzoAz1gwsaqAosTy0Joa
            PosbVLMPYXAvePR6Tz98vLUkGhIrZAFUxVSfUqKCCD9WhZ5gdAtPL
            by88p2iJG/Vzd6Y1JwDbe1l80GuxDf/z0Z+mhErx6Y/teBIcGENsS
            ysohOu65/i/3Ezu4CfKBdxKYx61BSBRrDHBqcb3Q3SUjI+Btg3iJ3
            ao26ZR+7Pb4qxCkrn5aEf+oHsUqNS2zpxXo4MEy0S0Tnn4KYCvtkW
            m6/mHuWgqC/IYnFmDff4T+rngkgRQKqJ9eCbOMjqZCTY+UwvNHGxd
            upnmHmiDDChB025QJJjCvSQbGA5p1FeKGUkfFb37VX0KpzoB0D7Us
            KMu2lQxhCyS92dHd94ytlBFhMsFmduiz69IU1EosIEHqE2LiRjcAa
            ZKPxOurKP7r+MwvUNbxSYfARrib9oWgj2YS+W27mZ5IAiGvPchuIM
            5yZ2uWgzOQdKhr5z8WUt2YF7g5hkcOwFY8krrMElqXEudAJv0CdW0
            dbQYg3mR4gbcNSgsg7w/iPlkRI/XIoxmlokjkO+wiZ1BJsE9kwSzU
            olGKL9c/YPVGmtQjFS47DA/HmaELwZBUZl1ZCZ6EGrIeZQ6Dr/ZkK
            XDpS2yOMAn3h3IKHT52dxO+Efb6YdELU7Bm8D3gL5TwvbjBcKDaf4
            GiZMTyGdw+ZH795Yuoj/F2HciMwqDTmrt/OFV5APjbZLx6FJrbC0r
            AtrgGy54AMVDZMJnzZuc8SGgl8AN1u51zEr3b+KCGDunOYoLQZhs7
            0IYDSOZmEBLFVUGNUgeG3p2At1OAnwpblRLg+Xw21JXNlk3KUYicK
            uJaNkGRmKGxGhG4lFZhi/JZiwuBvCrPZd3CjUzDJ0JZPZDHgkAf7Y
            5XOwdkrTElMCMGCSqGSIb3DQEJFTEWBBQAFBOqYFJlbkBoqPfCMK5
            F1BXODDAxMCEwCQYFKw4DAhoFAAQUhxd6YPi7JKB/24dSls9gKO/D
            HVoECHap2RUyKvQTAgIIAA==

            PayloadIdentifier
            com.example.mypkcs12payload
            PayloadType
            com.apple.security.pkcs12
            PayloadUUID
            C9BF4927-E819-4521-88DE-2AEB6E1DC3D8
            PayloadVersion
            1

    PayloadDisplayName
    App-Layer VPN
    PayloadIdentifier
    com.example.myprofile.applayervpn
    PayloadType
    Configuration
    PayloadUUID
    D95CCE2A-F0A7-4687-B03E-5784F3F0F575
    PayloadVersion
    1

```

## See Also

### VPN

object AppToAppLayerVPNMapping

The payload you use to configure per-app VPN settings.

object VPN

The payload you use to configure a VPN.

