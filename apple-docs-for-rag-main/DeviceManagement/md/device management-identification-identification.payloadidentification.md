

- Device Management
- Identification
-  Identification.PayloadIdentification 

Device Management Profile

# Identification.PayloadIdentification

The dictionary containing details about the user.

macOS 10.7–15.4DeprecatedDevice Assignment ServicesVPP License Management

``` source
object Identification.PayloadIdentification
```

## Properties

`AuthMethod`

`string`

Deprecated   (Required) 

The authorization method. Either the profile contains the password or the user provides it.

Possible Values: `Password, UserEnteredPassword`

`EmailAddress`

`string`

Deprecated   (Required) 

The address for the account.

`FullName`

`string`

Deprecated   (Required) 

The full name of the account.

`Password`

`string`

Deprecated   (Required) 

The password for the account. Required when the `AuthMethod` is `Password`.

`Prompt`

`string`

Deprecated 

The custom instructions for the user, if needed.

`PromptMessage`

`string`

Deprecated 

The additional descriptive text for the user prompt.

`UserName`

`string`

Deprecated   (Required) 

The UNIX user name for the accounts.

