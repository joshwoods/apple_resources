

- Device Management
- InstallApplicationCommand
-  InstallApplicationCommand.Command 

Device Management Command

# InstallApplicationCommand.Command

The request dictionary to install an app.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallApplicationCommand.Command
```

## Properties

`Attributes`

InstallApplicationCommand.Command.Attributes

A dictionary that contains the initial attributes of the app, if you choose to provide it. Available in iOS 7 and later, and tvOS 10.2 and later.

`ChangeManagementState`

`string`

The change management state. This value doesn’t work with the User Enrollment feature introduced in iOS 13. Available in iOS 9 and later, macOS 11 and later, and tvOS 10.2 and later. The only possible value is:

`Managed`  
Take management of the app if the user installed it already and `InstallAsManaged` is `true`.

Value: `Managed`

`Configuration`

InstallApplicationCommand.Command.Configuration

A dictionary that contains the initial configuration of the app, if you choose to provide it. Available in iOS 7 and later, macOS 11 and later, and tvOS 10.2 and later.

`Identifier`

`string`

The app’s bundle identifier.

Important

For a watchOS app, the identifier needs to be the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired. Obtain the watch’s bundle identifier for an app with a watch bundle, in the `watchBundleId` key that’s part of the Content Metadata query. For more information on this query, see Getting App and Book Information (Legacy).

`InstallAsManaged`

`boolean`

If `true`, install the app as a managed app. Otherwise, the system installs the app as unmanaged. If you reinstall a manged app and omit this value or set it to `false`, the app becomes unmanaged.

For manifest-based installs, if `true`, the system only considers apps installed in `/Applications` as managed. In macOS 11 through 13, the system requires that the `pkg` only contains a single signed app.

Available in macOS 11 and later.

Default: `false`

`iOSApp`

`boolean`

If `true`, the app is an iOS app that can run on an Apple silicon in macOS 11 and later.

Default: `false`

`iTunesStoreID`

`integer`

The app’s iTunes Store identifier.

`ManagementFlags`

`integer`

A bitwise OR of the management flags. The possible values are:

- `1`: If `InstallAsManaged` is `true`, remove the app upon removal of the MDM profile.

- `4`: Prevent backup of app data.

- `5`: Both `1` and `4`.

Available in iOS 5 and later, macOS 11 and later, and tvOS 10.2 and later.

Possible Values: `1, 4, 5`

`ManifestURL`

`string`

The URL of the app manifest, which needs to begin with `https:`.

`Options`

InstallApplicationCommand.Command.Options

A dictionary that contains the app installation options.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device needs to be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to install an app.

Value: `InstallApplication`

## Topics

### Commands

object InstallApplicationCommand.Command.Attributes

A dictionary that contains the initial attributes of the app.

object InstallApplicationCommand.Command.Configuration

A dictionary that contains the configuration to install an enterprise app.

object ManifestURL.ItemsItem

object InstallApplicationCommand.Command.Options

A dictionary that contains the app installation options.

