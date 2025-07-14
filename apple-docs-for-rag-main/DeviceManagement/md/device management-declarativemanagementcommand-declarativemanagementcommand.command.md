

- Device Management
- DeclarativeManagementCommand
-  DeclarativeManagementCommand.Command 

Device Management Command

# DeclarativeManagementCommand.Command

The command to enable the declarative management engine on a device.

iOS 15.0+iPadOS 15.0+macOS 13.0+tvOS 16.0+visionOS 1.1+watchOS 10.0+Device Assignment ServicesVPP License Management

``` source
object DeclarativeManagementCommand.Command
```

## Properties

`Data`

`data`

The base64-encoded Declarative Management JSON request using a TokensResponse.

`RequestRequiresNetworkTether`

`boolean`

If `true`, the device must be network-tethered to run the command.

Default: `false`

`RequestType`

`string`

 (Required) 

The request type to issue declarative commands on a device.

Value: `DeclarativeManagement`

## Discussion

The server uses this command to turn on the declarative management engine on the device the first time the server sends it. Subsequent commands trigger a declarative management synchronization operation.

