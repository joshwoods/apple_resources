

- Device Management
-  ExtensibleSingleSignOn 

Device Management Profile

# ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

iOS 13.0+iPadOS 13.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ExtensibleSingleSignOn
```

## Properties

`AuthenticationMethod`

`string`

Deprecated 

The Platform SSO authentication method the extension uses. Requires that the SSO Extension also supports the method. Available in macOS 13 and later, and deprecated in macOS 14.

Possible Values: `Password, UserSecureEnclaveKey`

`DeniedBundleIdentifiers`

`[string]`

An array of bundle identifiers of apps that don’t use SSO provided by this extension. Available in iOS 15 and later, and macOS 12 and later.

`ExtensionData`

ExtensibleSingleSignOn.ExtensionData

A dictionary of arbitrary data passed through to the app extension.

`ExtensionIdentifier`

`string`

 (Required) 

The bundle identifier of the app extension that performs SSO for the specified URLs.

`Hosts`

`[string]`

An array of host or domain names that apps can authenticate through the app extension.

Required for `Credential` payloads. Ignored for `Redirect` payloads.

The system:

- Matches host or domain names case-insensitively

- Requires that all the host and domain names of all installed Extensible SSO payloads are unique

Note

Host names that begin with a “.” are wildcard suffixes that match all subdomains; otherwise the host name needs be an exact match.

`PlatformSSO`

ExtensibleSingleSignOn.PlatformSSO

The dictionary to configure Platform SSO.

`Realm`

`string`

The realm name for `Credential` payloads. Use proper capitalization for this value. Ignored for `Redirect` payloads.

`RegistrationToken`

`string`

The token this device uses for registration with Platform SSO. Use it for silent registration with the Identity Provider. Requires that `AuthenticationMethod` isn’t empty. Available in macOS 13 and later.

`ScreenLockedBehavior`

`string`

If set to `Cancel`, the system cancels authentication requests when the screen is locked. If set to `DoNotHandle`, the request continues without SSO instead. This doesn’t apply to requests where `userInterfaceEnabled` is `false`, or for background URLSession requests. Available in iOS 15 and later, and macOS 12 and later.

Default: `Cancel`

Possible Values: `Cancel, DoNotHandle`

`TeamIdentifier`

`string`

The team identifier of the app extension. This key is required on macOS and ignored elsewhere.

`Type`

`string`

 (Required) 

The type of SSO.

Possible Values: `Credential, Redirect`

`URLs`

`[string]`

An array of URL prefixes of identity providers where the app extension performs SSO.

Required for `Redirect` payloads. Ignored for `Credential` payloads.

The URLs need to begin with `http://` or `https://`.

The system:

- Matches scheme and host name case-insensitively

- Doesn’t allow query parameters and URL fragments

- Requires that the URLs of all installed Extensible SSO payloads are unique

## Discussion

Specify `com.apple.extensiblesso` as the payload type.

The system supports user channel installation in macOS 11 and later.

### Profile Availability

|                            |                         |
|----------------------------|-------------------------|
| Device Channel             | macOS                   |
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
            com.example.com
            TeamIdentifier
            RandomTeamID
            Hosts

                .com.example.com

            Realm
            COM.URL.COM
            Type
            Credential
            PayloadIdentifier
            com.example.myessopayload
            PayloadType
            com.apple.extensiblesso
            PayloadUUID
            dbed949d-39a2-440d-a84b-e0c825cdcb2e
            PayloadVersion
            1

    PayloadDisplayName
    Extensible SSO
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    da3bbbec-a753-4aa7-aeae-a74b7a65c0b5
    PayloadVersion
    1

```

## Topics

### Supporting Objects

object ExtensibleSingleSignOn.ExtensionData

The additional data to pass to the app extension.

object ExtensibleSingleSignOn.PlatformSSO

The dictionary to configure Platform SSO.

## See Also

### Authentication

object DirectoryService

The payload you use to configure an Active Directory (AD) domain.

object ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

object Identification

The payload you use to configure the names of the account user.

object IdentityPreference

The payload you use to configure the user’s identity on the device.

object SingleSignOn

The payload you use to configure single sign-on (SSO).

