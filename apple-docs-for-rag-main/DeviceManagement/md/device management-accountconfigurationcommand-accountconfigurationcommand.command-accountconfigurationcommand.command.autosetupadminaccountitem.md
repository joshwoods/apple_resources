

- Device Management
- AccountConfigurationCommand
- AccountConfigurationCommand.Command
-  AccountConfigurationCommand.Command.AutoSetupAdminAccountItem 

Device Management Command

# AccountConfigurationCommand.Command.AutoSetupAdminAccountItem

A dictionary that describes the administrator account to create with Setup Assistant, which uses the first element and ignores additional elements.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object AccountConfigurationCommand.Command.AutoSetupAdminAccountItem
```

## Properties

`fullName`

`string`

The full name of the user, which defaults to `shortName` if not specified.

`hidden`

`boolean`

If `true`, this sets the account attribute to make the account hidden in the login window and Users & Groups.

Default: `false`

`passwordHash`

`data`

Data that contains the pre-created salted PBKDF2 SHA512 password hash for the account.

`shortName`

`string`

 (Required) 

The short name of the user.

## See Also

### Commands

object PasswordHash

A dictionary that contains the password hash for the account.

