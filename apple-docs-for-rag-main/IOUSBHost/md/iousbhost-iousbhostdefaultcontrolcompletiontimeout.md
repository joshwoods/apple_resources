

- IOUSBHost
-  IOUSBHostDefaultControlCompletionTimeout 

Global Variable

# IOUSBHostDefaultControlCompletionTimeout

The default completion timeout for input/output requests.

Mac Catalyst 14.0+macOS 10.15+

``` source
let IOUSBHostDefaultControlCompletionTimeout: TimeInterval
```

## See Also

### Sending Device Requests

func IOUSBHostDeviceRequestType(tIOUSBDeviceRequestDirectionValue, tIOUSBDeviceRequestTypeValue, tIOUSBDeviceRequestRecipientValue) -> UInt8

Creates the request type field of a device request.

