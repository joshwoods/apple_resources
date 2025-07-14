

- Device Management
- InstallApplicationCommand
- InstallApplicationCommand.Command
-  InstallApplicationCommand.Command.Options 

Device Management Command

# InstallApplicationCommand.Command.Options

A dictionary that contains the app installation options.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallApplicationCommand.Command.Options
```

## Properties

`PurchaseMethod`

`integer`

The app’s purchase type, which must be one of the following values:

- `0`: Free apps and Legacy Volume Purchase Program (VPP) with a redemption code. This option is only available in iOS.

- `1`: Volume Purchase Program (VPP) app assignment.

Set this value to `1` to install first-party apps without user login to the iTunes Store, such as Mail or Safari, or to install an iOS app with user enrollment.

Default: `0`

Possible Values: `0, 1`

## See Also

### Commands

object InstallApplicationCommand.Command.Attributes

A dictionary that contains the initial attributes of the app.

object InstallApplicationCommand.Command.Configuration

A dictionary that contains the configuration to install an enterprise app.

object ManifestURL.ItemsItem

