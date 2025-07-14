

- Device Management
-  StatusAppManagedListManagedConfigurationStateObject 

Object

# StatusAppManagedListManagedConfigurationStateObject

A dictionary that contains details about a declarative managed app’s managed configuration.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object StatusAppManagedListManagedConfigurationStateObject
```

## Properties

`state`

`string`

 (Required) 

The managed configuration status.

- `unknown` - the managed configuration has not been read

- `invalid` - the managed configuration was read and deemed to be invalid

- `valid` - the managed configuration was read and deemed to be valid

Possible Values: `unknown, invalid, valid`

## See Also

### Objects

object StatusAppManagedListManagedConfiguration_ExtensionConfigStateObject

A dictionary that contains details about a declarative managed app extension’s managed configuration.

