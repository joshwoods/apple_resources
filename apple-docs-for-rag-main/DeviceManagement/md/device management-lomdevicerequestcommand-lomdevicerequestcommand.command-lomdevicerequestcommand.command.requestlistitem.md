

- Device Management
- LOMDeviceRequestCommand
- LOMDeviceRequestCommand.Command
-  LOMDeviceRequestCommand.Command.RequestListItem 

Device Management Command

# LOMDeviceRequestCommand.Command.RequestListItem

A dictionary that contains a requested action to perform on a device using lights-out management (LOM).

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMDeviceRequestCommand.Command.RequestListItem
```

## Properties

`DeviceDNSName`

`string`

 (Required) 

The DNS name of the device. This should match the `dNSName` in SCEP.PayloadContent.SubjectAltName or an equivalent in a PKCS12 identity.

`DeviceRequestType`

`string`

 (Required) 

The requested action to perform on the device.

Possible Values: `PowerON, PowerOFF, Reset`

`DeviceRequestUUID`

`string`

 (Required) 

The unique identifier of the request.

`LOMProtocolVersion`

`integer`

 (Required) 

The LOM protocol version that the device supports. Provide the same value that `LOMProtocolVersion` receives in the LOMSetupRequestResponse.

`PrimaryIPv6AddressList`

`[string]`

 (Required) 

An array that contains the IPv6 addresses for primary LOM-compatible Ethernet interfaces for the device.

`SecondaryIPv6AddressList`

`[string]`

 (Required) 

An array that contains the IPv6 addresses for secondary LOM-compatible Ethernet interfaces for the device.

