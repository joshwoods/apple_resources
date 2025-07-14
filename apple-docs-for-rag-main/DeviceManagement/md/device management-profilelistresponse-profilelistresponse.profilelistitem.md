

- Device Management
- ProfileListResponse
-  ProfileListResponse.ProfileListItem 

Device Management Command

# ProfileListResponse.ProfileListItem

A dictionary that describes a profile list item.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ProfileListResponse.ProfileListItem
```

## Properties

`HasRemovalPasscode`

`boolean`

If `true`, the profile has a passcode for removal.

Default: `false`

`IsEncrypted`

`boolean`

If `true`, it’s an encrypted profile.

Default: `false`

`IsManaged`

`boolean`

If `true`, the current MDM service installed the profile. MDM doesn’t return this value for supervised devices, and can remove or replace all profiles on supervised devices.

Default: `false`

`PayloadContent`

`[`ProfileListResponse.ProfileListItem.PayloadContentItem`]`

An array of payload content items. This value isn’t present if `IsEncrypted` is `true`.

`PayloadDescription`

`string`

The description of the profile.

`PayloadDisplayName`

`string`

The human-readable name of the profile.

`PayloadIdentifier`

`string`

 (Required) 

The reverse-DNS-style identifier of the profile; for example, `com.example.myprofile`.

`PayloadOrganization`

`string`

The human-readable name of the organization that provided the profile.

`PayloadRemovalDisallowed`

`boolean`

If `true`, the user can’t delete the profile unless it has a removal password and the user provides it. The framework ignores this field on unsupervised devices.

Default: `false`

`PayloadUUID`

`string`

 (Required) 

The unique identifier for the profile.

`PayloadVersion`

`integer`

The version of the configuration profile as a whole, not of the individual profiles within it. The value should be `1`.

`SignerCertificates`

`[data]`

An array that contains the certificate for signing the profile, followed by any intermediate certificates, in DER-encoded X.509 format.

`Source`

`string`

## Mentioned in 

Dealing with Inactive MDM Devices and Invalid Push Tokens

## Topics

### Objects

object ProfileListResponse.ProfileListItem.PayloadContentItem

A dictionary that describes a profile payload content item.

## See Also

### Commands

object ProfileListResponse.ProfileListItem.PayloadContentItem

A dictionary that describes a profile payload content item.

object ProfileListResponse.ErrorChainItem

A dictionary that describes an error chain item.

