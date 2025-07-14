

- Device Management
-  StatusAppManagedListManagedConfigurationObject 

Object

# StatusAppManagedListManagedConfigurationObject

A dictionary that contains details about a declarative managed app’s managed configuration.

iOS 17.2+iPadOS 17.2+visionOS 2.4+Device Assignment ServicesVPP License Management

``` source
object StatusAppManagedListManagedConfigurationObject
```

## Properties

`app-config-state`

StatusAppManagedListManagedConfigurationStateObject

The status of any app managed configuration. This key is only present when the managed app has a managed configuration.

`extension-config-state`

StatusAppManagedListManagedConfiguration_ExtensionConfigStateObject

The status of any app extension managed configuration. This key’s value is a dictionary whose keys are the bundle identifiers of app extensions that have a managed configuration. The values of each key represent the status of the corresponding app extension’s managed configuration.

## Topics

### Objects

object StatusAppManagedListManagedConfigurationStateObject

A dictionary that contains details about a declarative managed app’s managed configuration.

object StatusAppManagedListManagedConfiguration_ExtensionConfigStateObject

A dictionary that contains details about a declarative managed app extension’s managed configuration.

## See Also

### Objects

object StatusAppManagedListStatusReasonObject

A dictionary that contains details about a declarative managed app’s state.

