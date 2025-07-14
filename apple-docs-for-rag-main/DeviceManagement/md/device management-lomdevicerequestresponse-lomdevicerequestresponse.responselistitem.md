

- Device Management
- LOMDeviceRequestResponse
-  LOMDeviceRequestResponse.ResponseListItem 

Device Management Command

# LOMDeviceRequestResponse.ResponseListItem

A dictionary that describes a response list item.

macOS 11.0+Device Assignment ServicesVPP License Management

``` source
object LOMDeviceRequestResponse.ResponseListItem
```

## Properties

`DeviceRequestReturnError`

`string`

If present, a description of the error for a failed request.

`DeviceRequestSuccess`

`boolean`

 (Required) 

If `true`, the request was successful.

`DeviceRequestUUID`

`string`

 (Required) 

The unique identifier of the request for this response list item.

## See Also

### Commands

object LOMDeviceRequestResponse.ErrorChainItem

A dictionary that describes an error chain item.

