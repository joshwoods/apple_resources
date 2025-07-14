

- Device Management
- InstallApplicationCommand
- InstallApplicationCommand.Command
-  InstallApplicationCommand.Command.Attributes 

Device Management Command

# InstallApplicationCommand.Command.Attributes

A dictionary that contains the initial attributes of the app.

iOS 5.0+iPadOS 5.0+macOS 10.9+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object InstallApplicationCommand.Command.Attributes
```

## Properties

`AssociatedDomains`

`[string]`

An array that contains the associated domains to add to this app. Available in iOS 13 and later.

`AssociatedDomainsEnableDirectDownloads`

`boolean`

If `true`, perform claimed site association verification directly at the domain instead of on Apple’s servers. Only set this to `true` for domains that can’t access the internet. Available in iOS 14 and later.

Default: `false`

`CellularSliceUUID`

`string`

The data network name (DNN) or app category. For DNN, the value is `DNN:name`, where `name` is the carrier-provided DNN name. For app category, the value is `AppCategory:category`, where `category` is a carrier-provided string like “Enterprise1”.

Available in iOS 17 and later.

`ContentFilterUUID`

`string`

The content filter UUID for this app. Available in iOS 16 and later.

`DNSProxyUUID`

`string`

The DNS proxy UUID for this app. Available in iOS 16 and later.

`Hideable`

`boolean`

Default: `true`

`Lockable`

`boolean`

Default: `true`

`RelayUUID`

`string`

The relay UUID for this app. Available in iOS 17 and later.

`Removable`

`boolean`

If `false`, this app isn’t removable while it’s a managed app. Available in iOS 14 and later, and tvOS 14 and later.

Default: `true`

`TapToPayScreenLock`

`boolean`

If `true`, Tap to Pay on iPhone requires users to use Face ID or a passcode to unlock their device after every transaction that requires a customer’s card PIN. If `false`, the user can configure this setting on their device.

Available in iOS 16.4 and later.

Default: `false`

`VPNUUID`

`string`

A per-app VPN unique identifier for this app. Available in iOS 7 and later, and tvOS 10.2 and later.

## See Also

### Commands

object InstallApplicationCommand.Command.Configuration

A dictionary that contains the configuration to install an enterprise app.

object ManifestURL.ItemsItem

object InstallApplicationCommand.Command.Options

A dictionary that contains the app installation options.

