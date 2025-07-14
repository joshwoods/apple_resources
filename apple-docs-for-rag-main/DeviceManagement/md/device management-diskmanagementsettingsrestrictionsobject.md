

- Device Management
-  DiskManagementSettingsRestrictionsObject 

Object

# DiskManagementSettingsRestrictionsObject

The restrictions for the disk.

macOS 15.0+Device Assignment ServicesVPP License Management

``` source
object DiskManagementSettingsRestrictionsObject
```

## Properties

`ExternalStorage`

`string`

Specifies the mount policy for external storage:

- `Allowed`: the system can mount external storage that is read-write or read-only.

- `ReadOnly`: the system can only mount read-only external storage. Note that external storage that is read-write will not be mounted read-only.

- `Disallowed`: The system can’t mount any external storage.

Possible Values: `Allowed, ReadOnly, Disallowed`

`NetworkStorage`

`string`

Specifies the mount policy for network storage:

- `Allowed`: the system can mount network storage that is read-write or read-only.

- `ReadOnly`: the system can only mount read-only network storage. Note that network storage that is read-write will not be mounted read-only.

- `Disallowed`: The system can’t mount any network storage.

Possible Values: `Allowed, ReadOnly, Disallowed`

