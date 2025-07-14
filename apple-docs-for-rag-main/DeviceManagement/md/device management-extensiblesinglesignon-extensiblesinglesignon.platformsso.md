

- Device Management
- ExtensibleSingleSignOn
-  ExtensibleSingleSignOn.PlatformSSO 

Device Management Profile

# ExtensibleSingleSignOn.PlatformSSO

The dictionary to configure Platform SSO.

iOS 13.0+iPadOS 13.0+macOS 10.15+visionOS 1.1+Device Assignment ServicesVPP License Management

``` source
object ExtensibleSingleSignOn.PlatformSSO
```

## Properties

`AccountDisplayName`

`string`

The display name for the account in notifications and authentication requests.

`AdditionalGroups`

`[string]`

The list of created groups that don’t have administrator access.

`AdministratorGroups`

`[string]`

The list of groups to use for administrator access. The system requests membership during authentication.

`AuthenticationGracePeriod`

`integer`

The amount of time after a `FileVaultPolicy`, `LoginPolicy`, or `UnlockPolicy` is received or updated that unregistered local accounts can be used. Required when `AllowAuthenticationGracePeriod` is set. Available in macOS 15 and later.

`AuthenticationMethod`

`string`

The Platform SSO authentication method to use with the extension. Requires that the SSO Extension also support the method.

Possible Values: `Password, UserSecureEnclaveKey, SmartCard`

`AuthorizationGroups`

ExtensibleSingleSignOn.PlatformSSO.AuthorizationGroups

The pairing of Authorization Rights to group names. The system updates the Authorization Right to use the group when used.

`EnableAuthorization`

`boolean`

Enables using identity provider accounts at authorization prompts. Requires that `UseSharedDeviceKeys` is `true`. The system assigns groups using `AdministratorGroups`, `AdditionalGroups`, or `AuthorizationGroups`.

Default: `false`

`EnableCreateUserAtLogin`

`boolean`

Enables creating new users at the login window with an `AuthenticationMethod` of either `Password` or `SmartCard`. Requires that `UseSharedDeviceKeys` is `true`.

Default: `false`

`FileVaultPolicy`

`[string]`

The policy to apply when using Platform SSO at FileVault unlock on Apple Silicon Macs. Applies when `AuthenticationMethod` is `Password`. Available in macOS 15 and later.

Possible Values: `AttemptAuthentication, RequireAuthentication, AllowOfflineGracePeriod, AllowAuthenticationGracePeriod`

`LoginFrequency`

`integer`

The duration, in seconds, until the system requires a full login instead of a refresh. The default value is 64,800 (18 hours). The minimum value is 3600 (1 hour).

Default: `64800`

Minimum: `3600`

`LoginPolicy`

`[string]`

The policy to apply when using Platform SSO at the login window. Applies when `AuthenticationMethod` is `Password`. Available in macOS 15 and later.

Possible Values: `AttemptAuthentication, RequireAuthentication, AllowOfflineGracePeriod, AllowAuthenticationGracePeriod`

`NewUserAuthorizationMode`

`string`

The permission to apply to newly created accounts at login. Allowed values:

`Standard`  
The account is a standard user.

`Admin`  
The system adds the account to the local administrators group.

`Groups`  
The system assigns group to the account using `AdministratorGroups`, `AdditionalGroups`, or `AuthorizationGroups`.

Possible Values: `Standard, Admin, Groups`

`NonPlatformSSOAccounts`

`[string]`

The list of local accounts that aren’t subject to the `FileVaultPolicy`, `LoginPolicy`, or `UnlockPolicy`. The accounts aren’t prompted to register for Platform SSO. Available in macOS 15 and later.

`OfflineGracePeriod`

`integer`

The amount of time after the last successful Platform SSO login a local account password can be used offline. Required when `AllowOfflineGracePeriod` is set. Available in macOS 15 and later.

`TokenToUserMapping`

ExtensibleSingleSignOn.PlatformSSO.TokenToUserMapping

The attribute mapping to use when creating new users or for authorization.

`UnlockPolicy`

`[string]`

The policy to apply when using Platform SSO at screensaver unlock. Applies when `AuthenticationMethod` is `Password`. Available in macOS 15 and later.

Possible Values: `AttemptAuthentication, RequireAuthentication, AllowOfflineGracePeriod, AllowAuthenticationGracePeriod, AllowTouchIDOrWatchForUnlock`

`UserAuthorizationMode`

`string`

The permission to apply to an account each time the user authenticates. Allowed values:

`Standard`  
The account is a standard user.

`Admin`  
The system adds the account to the local administrators group.

`Groups`  
The system assigns group to the account using `AdministratorGroups`, `AdditionalGroups`, or `AuthorizationGroups`.

Possible Values: `Standard, Admin, Groups`

`UseSharedDeviceKeys`

`boolean`

If `true`, the system uses the same signing and encryption keys for all users.

Default: `false`

`AllowDeviceIdentifiersInAttestation`

`boolean`

Default: `false`

## Topics

### Supporting Objects

object ExtensibleSingleSignOn.PlatformSSO.AuthorizationGroups

The pairing of Authorization Rights to group names.

object ExtensibleSingleSignOn.PlatformSSO.TokenToUserMapping

The attribute mapping to use when creating new users or for authorization.

## See Also

### Supporting Objects

object ExtensibleSingleSignOn.ExtensionData

The additional data to pass to the app extension.

