

- Device Management
-  PasswordHash 

Object

# PasswordHash

A dictionary that contains the password hash for the account.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object PasswordHash
```

## Properties

`SALTED-SHA512-PBKDF2`

PasswordHash.SALTED-SHA512-PBKDF2

 (Required) 

A dictionary that contains the `entropy`, `iterations`, and `salt` elements to create the password hash using the CommonCrypto libraries, or equivalent. Convert this dictionary to binary data before setting it as the value for the password hash.

## Topics

### Objects

object PasswordHash.SALTED-SHA512-PBKDF2

A dictionary that contains the elements you use to create the password hash.

## See Also

### Commands

object AccountConfigurationCommand.Command.AutoSetupAdminAccountItem

A dictionary that describes the administrator account to create with Setup Assistant, which uses the first element and ignores additional elements.

