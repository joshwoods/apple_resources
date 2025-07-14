

- IOUSBHost
-  IOUSBHostDeviceRequestType(\_:\_:\_:) 

Function

# IOUSBHostDeviceRequestType(\_:\_:\_:)

Creates the request type field of a device request.

Mac Catalyst 14.0+macOS 10.15+

``` source
func IOUSBHostDeviceRequestType(
    _ direction: tIOUSBDeviceRequestDirectionValue,
    _ type: tIOUSBDeviceRequestTypeValue,
    _ recipient: tIOUSBDeviceRequestRecipientValue
) -> UInt8
```

## Parameters 

`direction`  

The direction of the request.

`type`  

The type of the request.

`recipient`  

The recipient of the request.

## Return Value

The request type.

## See Also

### Sending Device Requests

let IOUSBHostDefaultControlCompletionTimeout: TimeInterval

The default completion timeout for input/output requests.

