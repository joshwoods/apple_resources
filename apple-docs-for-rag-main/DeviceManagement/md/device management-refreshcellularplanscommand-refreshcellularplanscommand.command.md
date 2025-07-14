

- Device Management
- RefreshCellularPlansCommand
-  RefreshCellularPlansCommand.Command 

Device Management Command

# RefreshCellularPlansCommand.Command

The request dictionary to query a carrier URL for active eSIM cellular-plan profiles.

iOS 13.0+iPadOS 13.0+Device Assignment ServicesVPP License Management

``` source
object RefreshCellularPlansCommand.Command
```

## Properties

`eSIMServerURL`

`string`

 (Required) 

The carrier’s eSIM server URL to query. Obtain this URL from each carrier separately.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to query a carrier URL for active eSIM cellular-plan profiles.

Value: `RefreshCellularPlans`

