

- Device Management
- PrivacyPreferencesPolicyControl
- PrivacyPreferencesPolicyControl.Services
-  PrivacyPreferencesPolicyControl.Services.Identity 

Device Management Profile

# PrivacyPreferencesPolicyControl.Services.Identity

A dictionary listing apps and the privacy policy to apply to them.

macOS 10.14+Device Assignment ServicesVPP License Management

``` source
object PrivacyPreferencesPolicyControl.Services.Identity
```

## Properties

`AEReceiverCodeRequirement`

`string`

The code requirement for the receiving binary. This code requirement is required for AppleEvents service; not valid for other services.

`AEReceiverIdentifier`

`string`

The identifier of the process receiving an AppleEvent sent by the Identifier process. This identifier is required for AppleEvents service; not valid for other services.

`AEReceiverIdentifierType`

`string`

The type of AEReceiverIdentifier value, either `bundleID` or `path`. This setting is required for AppleEvents service; not valid for other services.

Possible Values: `bundleID, path`

`Allowed`

`boolean`

 (Required) 

If `true`, access is granted; otherwise, the process doesn’t have access. The user isn’t prompted and can’t change this value.

Note

Every payload needs to include either `Authorization` or `Allowed`, but not both.

`Authorization`

`string`

The `Authorization` key is an optional replacement for the `Allowed` key, which has one of the following possible values:

`Allow`  
Equivalent to a `true` value for the `Allowed` key

`Deny`  
Equivalent to a f`alse` value for the `Allowed` key

`AllowStandardUserToSetSystemService`  
Allows a standard (non-admin) user to configure the permissions for the specified app in the Privacy preferences for services that otherwise require admin authorization; only valid for the `ListenEvent` and `ScreenCapture` services

Note

Every payload needs to include either `Authorization` or `Allowed`, but not both.

Available in macOS 11 and later.

Possible Values: `Allow, Deny, AllowStandardUserToSetSystemService`

`CodeRequirement`

`string`

 (Required) 

Obtained via the command “`codesign -display -r -`”.

`Comment`

`string`

Not used.

`Identifier`

`string`

 (Required) 

The bundle ID or installation path of the binary.

`IdentifierType`

`string`

 (Required) 

The type of identifier value. Application bundles must be identified by bundle ID. Nonbundled binaries must be identified by installation path. Helper tools embedded within an application bundle automatically inherit the permissions of their enclosing app bundle.

Possible Values: `bundleID, path`

`StaticCode`

`boolean`

If `true`, statically validate the code requirement. Used only if the process invalidates its dynamic code signature.

Default: `false`

