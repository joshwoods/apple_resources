

- Device Management
- RemoveApplicationCommand
-  RemoveApplicationCommand.Command 

Device Management Command

# RemoveApplicationCommand.Command

The request dictionary to remove an installed managed app.

iOS 5.0+iPadOS 5.0+macOS 11.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object RemoveApplicationCommand.Command
```

## Properties

`Identifier`

`string`

 (Required) 

The bundle identifier of the managed app.

Important

`RequestRequiresNetworkTether`

`boolean`

Default: `false`

`RequestType`

`string`

 (Required) 

Value: `RemoveApplication`

## Overview

Note

For a watchOS app, the identifier needs to be the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired. Obtain the watch’s bundle identifier for an app with a watch bundle, in the `watchBundleId` key that’s part of the Content Metadata query. For more information on this query, see Getting App and Book Information (Legacy).

- RequestRequiresNetworkTether: If `true`, the device must be network-tethered to run the command.

- RequestType: The request type to remove an installed managed app.

