

- Device Management
-  ExtensibleSingleSignOnKerberos 

Device Management Profile

# ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

iOS 13.0+iPadOS 13.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ExtensibleSingleSignOnKerberos
```

## Properties

`ExtensionData`

ExtensibleSingleSignOnKerberos.ExtensionData

This is the dictionary used by the Apple built-in Kerberos extension.

`ExtensionIdentifier`

`string`

 (Required) 

Set this to `com.apple.AppSSOKerberos.KerberosExtension` for this extension.

Value: `com.apple.AppSSOKerberos.KerberosExtension`

`Hosts`

`[string]`

One or more host or domain names for which the app extension performs SSO.

The system:

- Matches host or domain names case-insensitively

- Requires that all the host and domain names of all installed Extensible SSO payloads are unique

Note

Host names that begin with a “.” are wildcard suffixes that match all subdomains; otherwise the host name needs be an exact match.

`Realm`

`string`

 (Required) 

The Kerberos realm. Use proper capitalization for this value. If in an Active Directory forest, this is the realm where the user logs in.

`Type`

`string`

 (Required) 

Set this to `Credential` for this extension.

Value: `Credential`

`TeamIdentifier`

`string`

 (Required) 

Set this to `apple` for this extension.

Value: `apple`

## Discussion

Specify `com.apple.extensiblesso` as the payload type.

This is a version of the profile that defines the specific keys and values needed for the Kerberos extension.

The system supports user channel installation in macOS 11 and later.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | iOS, macOS              |
| User Channel               | macOS, Shared iPad      |
| Allow Manual Install       | \-                      |
| Requires Supervision       | \-                      |
| Requires User Approved MDM | macOS                   |
| Allowed in User Enrollment | iOS, macOS              |
| Allow Multiple Payloads    | iOS, macOS, Shared iPad |

### Profile Example

```

    PayloadContent

            ExtensionData

                useSiteAutoDiscovery

            ExtensionIdentifier
            com.apple.Extension
            TeamIdentifier
            RandomTeamID
            Hosts

                url.example.com

            Realm
            COM.URL.COM
            Type
            Credential
            PayloadIdentifier
            com.example.myessokpayload
            PayloadType
            com.apple.extensiblesso
            PayloadUUID
            86c12312-c278-41f1-bbe7-9422a1e40ca2
            PayloadVersion
            1

    PayloadDisplayName
    Extensible SSO (Kerberos)
    PayloadIdentifier
    com.example.profile
    PayloadType
    Configuration
    PayloadUUID
    60bb7b2e-b94b-4f0d-848d-13c3a9857258
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object ExtensibleSingleSignOnKerberos.ExtensionData

The additional data to pass to the app extension.

## See Also

### Authentication

object DirectoryService

The payload you use to configure an Active Directory (AD) domain.

object ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

object Identification

The payload you use to configure the names of the account user.

object IdentityPreference

The payload you use to configure the user’s identity on the device.

object SingleSignOn

The payload you use to configure single sign-on (SSO).

