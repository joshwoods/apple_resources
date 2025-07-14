

- Device Management
- AccountConfigurationCommand
-  AccountConfigurationCommand.Command 

Device Management Command

# AccountConfigurationCommand.Command

The request dictionary to create a local administrator account.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object AccountConfigurationCommand.Command
```

## Properties

`AutoSetupAdminAccounts`

`[`AccountConfigurationCommand.Command.AutoSetupAdminAccountItem`]`

A dictionary that describes the administrator account to create with Setup Assistant, which uses the first element and ignores additional elements.

`DontAutoPopulatePrimaryAccountInfo`

`boolean`

If `true`, Setup Assistant ignores the primary account information and requires the user to enter that information. If `false`, Setup Assistant prefills the Full Name field with `PrimaryAccountFullName` and the User Name field with `PrimaryAccountUserName`. This value is available in macOS 10.15 and later.

Default: `false`

`LockPrimaryAccountInfo`

`boolean`

If `true`, and you provide values for `PrimaryAccountFullName` or `PrimaryAccountUserName`, Setup Assistant disables editing for the corresponding fields. `DontAutoPopulatePrimaryAccountInfo` must also be 0 (or missing).

If the user’s password is also available from authentication through ConfigurationURL, Setup Assistant automatically creates the primary account with that information and skips showing the user interface to view or edit these fields.

This value is available in macOS 10.15 and later.

Default: `false`

`ManagedLocalUserShortName`

`string`

If present, this is the short name of the local account to manage, which can also be the account that results from setting `AutoSetupAdminAccounts` to `true`. Otherwise, only the local account that Setup Assistant creates is a managed account. This value is available in macOS 11 and later.

`PrimaryAccountFullName`

`string`

The full name for the primary account. If present, Setup Assistant uses this value to prefill the Full Name field. However, Setup Assistant ignores this value if `DontAutoPopulatePrimaryAccountInfo` is `true`. This value is available in macOS 10.15 and later.

`PrimaryAccountUserName`

`string`

The account name for the primary account. If present, Setup Assistant uses this value to prefill the User Name field. However, Setup Assistant ignores this value if `DontAutoPopulatePrimaryAccountInfo` is `true`. This value is available in macOS 10.15 and later.

`RequestType`

`string`

 (Required) 

The request type to create a local administrator account.

Value: `AccountConfiguration`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`SetPrimarySetupAccountAsRegularUser`

`boolean`

If `true`, Setup Assistant creates the primary accounts as regular users, and you must specify a value for `AutoSetupAdminAccounts`.

Default: `false`

`SkipPrimarySetupAccountCreation`

`boolean`

If `true`, Setup Assistant skips the user interface for setting up primary accounts and disables autologin. If `true`, you must specify a value for `AutoSetupAdminAccounts`.

Default: `false`

## Topics

### Commands

object AccountConfigurationCommand.Command.AutoSetupAdminAccountItem

A dictionary that describes the administrator account to create with Setup Assistant, which uses the first element and ignores additional elements.

object PasswordHash

A dictionary that contains the password hash for the account.

