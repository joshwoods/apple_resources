

- Device Management
-  DirectoryService 

Device Management Profile

# DirectoryService

The payload you use to configure an Active Directory (AD) domain.

macOS 10.8+Device Assignment ServicesVPP License Management

``` source
object DirectoryService
```

## Properties

`ADAllowMultiDomainAuth`

`boolean`

If `true`, the system allows authentication from any domain in the namespace.

Default: `false`

`ADAllowMultiDomainAuthFlag`

`boolean`

If `true`, the system enables the `ADAllowMultiDomainAuth` key.

Default: `false`

`ADCreateMobileAccountAtLogin`

`boolean`

If `true`, the system creates a mobile account at login.

Default: `false`

`ADCreateMobileAccountAtLoginFlag`

`boolean`

If `true`, the system enables the `ADCreateMobileAccountAtLogin` key.

Default: `false`

`ADDefaultUserShell`

`string`

The default user shell.

`ADDefaultUserShellFlag`

`boolean`

If `true`, the system enables the `ADDefaultUserShell` key.

Default: `false`

`ADDomainAdminGroupList`

`[string]`

The list of Active Directory groups with admin access.

`ADDomainAdminGroupListFlag`

`boolean`

If `true`, the system enables the `ADDomainAdminGroupList` key.

Default: `false`

`ADForceHomeLocal`

`boolean`

If `true`, the system forces a local home directory.

Default: `false`

`ADForceHomeLocalFlag`

`boolean`

If `true`, the system enables the `ADForceHomeLocal` key.

Default: `false`

`ADMapGGIDAttribute`

`string`

The map group GID to attribute.

`ADMapGGIDAttributeFlag`

`boolean`

If `true`, the system enables the `ADMapGGIDAttributeFlag` key.

Default: `false`

`ADMapGIDAttribute`

`string`

The map GID to attribute.

`ADMapGIDAttributeFlag`

`boolean`

If `true`, the system enables the `ADMapGIDAttribute` key.

Default: `false`

`ADMapUIDAttribute`

`string`

The map UID to attribute.

`ADMapUIDAttributeFlag`

`boolean`

If `true`, the system enables the `ADMapUIDAttribute` key.

Default: `false`

`ADMountStyle`

`string`

The network home protocol to use: `afp` or `smb`.

`ADNamespace`

`string`

The primary user account naming convention; either `forest` or `domain`.

`ADNamespaceFlag`

`boolean`

If `true`, the system enables the `ADNamespace` key.

Default: `false`

`ADOrganizationalUnit`

`string`

The organizational unit to add the joining computer object to.

`ADPacketEncrypt`

`string`

The packet encryption policy.

`ADPacketEncryptFlag`

`boolean`

If `true`, the system enables the `ADPacketEncrypt` key.

Default: `false`

`ADPacketSign`

`string`

The packet signing policy.

`ADPacketSignFlag`

`boolean`

If `true`, the system enables the `ADPacketSign` key.

Default: `false`

`ADPreferredDCServer`

`string`

The preferred domain server.

`ADPreferredDCServerFlag`

`boolean`

If `true`, the system enables the `ADPreferredDCServer` key.

Default: `false`

`ADRestrictDDNS`

`[string]`

An array of strings that represent the interfaces allowed for dynamic DNS updates, such as en0 and en1.

`ADRestrictDDNSFlag`

`boolean`

If `true`, the system enables the `ADRestrictDDNS` key.

Default: `false`

`ADTrustChangePassIntervalDays`

`integer`

The number of days before requiring a change of the computer trust account password. Set to `0` to disable the feature.

`ADTrustChangePassIntervalDaysFlag`

`boolean`

If `true`, the system enables the `ADTrustChangePassIntervalDays` key.

Default: `false`

`ADUseWindowsUNCPath`

`boolean`

If `true`, the system uses the UNC path from Active Directory to derive the network home location.

Default: `false`

`ADUseWindowsUNCPathFlag`

`boolean`

If `true`, the system enables the `ADUseWindowsUNCPath` key.

Default: `false`

`ADWarnUserBeforeCreatingMA`

`boolean`

If `true`, the system enables the warning before creating the mobile account.

Default: `false`

`ADWarnUserBeforeCreatingMAFlag`

`boolean`

If `true`, the system enables the `ADWarnUserBeforeCreatingMA` key.

Default: `false`

`ClientID`

`string`

The client’s identifier.

`Description`

`string`

The directory service description.

`HostName`

`string`

 (Required) 

The Active Directory domain to join.

`Password`

`string`

The password of the account for the domain.

`UserName`

`string`

The user name of the account for the domain.

## Discussion

Specify `com.apple.DirectoryService.managed` as the payload type.

### Profile Availability

|                            |       |
|----------------------------|-------|
| Device Channel             | macOS |
| User Channel               | \-    |
| Allow Manual Install       | macOS |
| Requires Supervision       | \-    |
| Requires User Approved MDM | \-    |
| Allowed in User Enrollment | macOS |
| Allow Multiple Payloads    | macOS |

### Profile Example

```

    PayloadContent

            HostName
            host.example.com
            Password
            Password123
            UserName
            bind
            PayloadIdentifier
            com.example.mydspayload
            PayloadType
            com.apple.DirectoryService.managed
            PayloadUUID
            bb657e20-60b9-4c47-8730-51803ddf69e7
            PayloadVersion
            1

    PayloadDisplayName
    Active Directory
    PayloadIdentifier
    com.example.myprofile
    PayloadType
    Configuration
    PayloadUUID
    079b6bc3-4356-4d80-89b4-a4b8a82eb739
    PayloadVersion
    1

```

## See Also

### Authentication

object ExtensibleSingleSignOn

The payload you use to configure an app extension that performs single sign-on (SSO).

object ExtensibleSingleSignOnKerberos

The payload you use to configure an app extension that performs single sign-on with the Kerberos extension.

object Identification

The payload you use to configure the names of the account user.

object IdentityPreference

The payload you use to configure the user’s identity on the device.

object SingleSignOn

The payload you use to configure single sign-on (SSO).

