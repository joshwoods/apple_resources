

- Device Management
-  SingleSignOn 

Device Management Profile

# SingleSignOn

The payload you use to configure single sign-on (SSO).

iOS 7.0+iPadOS 7.0+Device Assignment ServicesVPP License Management

``` source
object SingleSignOn
```

## Properties

`Kerberos`

SingleSignOn.Kerberos

The Kerberos dictionary.

`Name`

`string`

 (Required) 

The human-readable name for the account.

## Discussion

Specify `com.apple.sso` as the payload type.

### Profile Availability

|                            |     |
|----------------------------|-----|
| Device Channel             | iOS |
| User Channel               | \-  |
| Allow Manual Install       | iOS |
| Requires Supervision       | \-  |
| Requires User Approved MDM | \-  |
| Allowed in User Enrollment | iOS |
| Allow Multiple Payloads    | \-  |

### Profile Example

```

    PayloadContent

            ExtensionData

                useSiteAutoDiscovery

            ExtensionIdentifier
            com.apple.com
            TeamIdentifier
            RandomTeamID
            Hosts

                .com.example.com

            Realm
            com.example.com
            Type
            Credential
            PayloadIdentifier
            com.example.myssopayload
            PayloadType
            com.apple.sso
            PayloadUUID
            02cdfc1c-3c53-434d-99db-c55ee62548bd
            PayloadVersion
            1

    PayloadDisplayName
    SSO
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    00d92c73-9844-4dc6-b742-eda33efbbf23
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object SingleSignOn.Kerberos

## See Also

### Authentication

object DirectoryService

The payload you use to configure an Active Directory (AD) domain.

object ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

object ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

object Identification

The payload you use to configure the names of the account user.

object IdentityPreference

The payload you use to configure the user’s identity on the device.

