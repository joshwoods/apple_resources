

- Device Management
-  AppManagedInstallBehaviorObject 

Object

# AppManagedInstallBehaviorObject

A dictionary that describes how and when to install an app.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
object AppManagedInstallBehaviorObject
```

## Properties

`Install`

`string`

A string that specifies if the app needs to remain on the device at all times or if the user can freely install and remove it, which is one of the following values:

Optional  
The user can install and remove the app after the system activates the configuration.

Required  
The system installs the app after it activates the configuration. The user can’t remove the app.

The system automatically installs apps on supervised devices. Otherwise, the device prompts the user to approve installation of the app.

Default: `Optional`

Possible Values: `Optional, Required`

`License`

AppManagedInstallBehavior_LicenseObject

A dictionary that describes the app’s license.

## Topics

### Objects

object AppManagedInstallBehavior_LicenseObject

A dictionary that specifies the type of license the app uses.

## See Also

### Objects

object AppManagedAppConfigDictionaryObject

A dictionary of app config data and credentials.

object AppManagedAttributesObject

A dictionary of values associated with an app.

object AppManagedCredentialConfigObject

A dictionary of values associated with a credential config.

object AppManagedExtensionConfigsObject

A dictionary of values associated with an extension config.

