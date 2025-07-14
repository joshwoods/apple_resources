

- Device Management
- SetAutoAdminPasswordCommand
-  SetAutoAdminPasswordCommand.Command 

Device Management Command

# SetAutoAdminPasswordCommand.Command

The request dictionary to change the password of a local administrator account.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object SetAutoAdminPasswordCommand.Command
```

## Properties

`GUID`

`string`

 (Required) 

The unique identifier of the local administrator account. If this value doesn’t match the GUID of an administrator account that MDM created during Device Enrollment Program (DEP) enrollment, the command returns an error.

`passwordHash`

`data`

 (Required) 

The precreated salted SHA-512 PBKDF2 password hash for the account.

Create this hash on the server using the CommonCrypto libraries, or equivalent, as a salted SHA-512 PBKDF2 dictionary that contains these elements:

- `entropy`: The derived key from the password hash; for example, from `CCKeyDerivationPBKDF()`

- `salt`: The 32-byte randomized salt; for example, from `CCRandomCopyBytes()`

- `iterations:` The number of iterations; for example, from `CCCalibratePBKDF()` using a minimum hash time of 100 milliseconds, or if unknown, a number in the range of 20,000 to 40,000 iterations

Place the dictionary that contains these elements into an outer dictionary with the key `SALTED-SHA512-PBKDF2`. Convert this dictionary to binary data before setting it as the value for `passwordHash`.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to change the password of a local administrator account.

Value: `SetAutoAdminPassword`

