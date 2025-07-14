

- Device Management
- ManagedApplicationAttributesCommand
-  ManagedApplicationAttributesCommand.Command 

Device Management Command

# ManagedApplicationAttributesCommand.Command

The request dictionary to query managed app attributes.

iOS 7.0+iPadOS 7.0+tvOS 10.2+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object ManagedApplicationAttributesCommand.Command
```

## Properties

`Identifiers`

`[string]`

 (Required) 

The bundle identifiers of the managed apps.

Important

`RequestRequiresNetworkTether`

`boolean`

Default: `false`

`RequestType`

`string`

 (Required) 

Value: `ManagedApplicationAttributes`

## Overview

Note

For a watchOS app, the identifier needs to be the watch’s bundle identifier, which differs from the main bundle identifier for the iPhone to which the watch is paired. Obtain the watch’s bundle identifier for an app with a watch bundle, in the `watchBundleId` key that’s part of the Content Metadata query. For more information on this query, see Getting App and Book Information (Legacy).

- RequestRequiresNetworkTether: If `true`, the device must be network-tethered to run the command.

- RequestType: The request type to query managed app attributes.

