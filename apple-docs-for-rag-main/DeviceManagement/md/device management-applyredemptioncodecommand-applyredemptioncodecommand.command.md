

- Device Management
- ApplyRedemptionCodeCommand
-  ApplyRedemptionCodeCommand.Command 

Device Management Command

# ApplyRedemptionCodeCommand.Command

The request dictionary to send a redemption code to complete installation of an app.

iOS 5.0+iPadOS 5.0+Device Assignment ServicesVPP License Management

``` source
object ApplyRedemptionCodeCommand.Command
```

## Properties

`Identifier`

`string`

 (Required) 

The bundle identifier of the app.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to send a redemption code.

Value: `ApplyRedemptionCode`

`RedemptionCode`

`string`

 (Required) 

The redemption code that applies to the app pending installation.

