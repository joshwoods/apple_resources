

- Device Management
- ScheduleOSUpdateScanCommand
-  ScheduleOSUpdateScanCommand.Command 

Device Management Command

# ScheduleOSUpdateScanCommand.Command

The request dictionary to schedule an operating-system update scan.

macOS 10.11+Device Assignment ServicesVPP License Management

``` source
object ScheduleOSUpdateScanCommand.Command
```

## Properties

`Force`

`boolean`

If `true`, force a scan to start immediately. Otherwise, the scan starts at a system-determined time.

Default: `false`

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to schedule an operating-system update scan.

Value: `ScheduleOSUpdateScan`

