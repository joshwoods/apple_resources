

- Device Management
- InstallEnterpriseApplicationCommand
-  InstallEnterpriseApplicationCommand.Command 

Device Management Command

# InstallEnterpriseApplicationCommand.Command

The request dictionary to install an enterprise app.

macOS 10.13.6+Device Assignment ServicesVPP License Management

``` source
object InstallEnterpriseApplicationCommand.Command
```

## Properties

`ChangeManagementState`

`string`

The change management state. This value doesn’t work with the User Enrollment feature introduced in iOS 13. The only possible value is:

`Managed`  
Take management of the app if the user installed it already and `InstallAsManaged` is `true`.

Available in macOS 11 and later.

Value: `Managed`

`Configuration`

InstallEnterpriseApplicationCommand.Command.Configuration

A dictionary that contains the initial configuration of the app, if you choose to provide it. Available in macOS 11 and later.

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

`ManagementFlags`

`integer`

The management flags. The possible values are:

`1`  
If `InstallAsManaged` is `true`, remove the app upon removal of the MDM profile.

Available in macOS 11 and later.

Value: `1`

`Manifest`

InstallEnterpriseApplicationCommand.Command.Manifest

A dictionary that specifies where to download the app. This value is backward-compatible with the manifest for the InstallApplicationCommand; however, it also allows you to specify `sha256s` and `sha256-size` for SHA-256 hashes.

`ManifestURL`

`string`

The URL of the app manifest, which needs to begin with `https:`.

`ManifestURLPinningCerts`

`[data]`

An array of DER-encoded certificates to pin the connection when fetching the `ManifestURL`.

`PinningRevocationCheckRequired`

`boolean`

If `true`, certificate revocation checks require a positive response when using certificate pinning with `ManifestURLPinningCerts`.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device needs to be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to install an enterprise managed app.

Value: `InstallEnterpriseApplication`

## Topics

### Commands

object InstallEnterpriseApplicationCommand.Command.Configuration

A dictionary that contains the configuration to install an enterprise app.

object InstallEnterpriseApplicationCommand.Command.Manifest

A dictionary that contains a manifest.

object ManifestURL

The URL to the app manifest.

object ManifestURL.ItemsItem.Metadata

