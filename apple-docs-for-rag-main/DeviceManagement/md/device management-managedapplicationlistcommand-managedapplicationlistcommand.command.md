

- Device Management
- ManagedApplicationListCommand
-  ManagedApplicationListCommand.Command 

Device Management Command

# ManagedApplicationListCommand.Command

The request dictionary to get the status of managed apps.

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationListCommand.Command
```

## Properties

`Identifiers`

`[string]`

The bundle identifiers of the managed apps to include in the response. For a watchOS app, the identifier needs to be the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired. Obtain the watch’s bundle identifier for an app with a watch bundle, in the `watchBundleId` key that’s part of the Content Metadata query. For more information on this query, see Getting App and Book Information (Legacy).

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to get the status of managed apps.

Value: `ManagedApplicationList`

