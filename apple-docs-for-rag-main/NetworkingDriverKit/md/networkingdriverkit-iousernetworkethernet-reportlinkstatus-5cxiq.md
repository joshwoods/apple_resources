

- NetworkingDriverKit
- IOUserNetworkEthernet
-  ReportLinkStatus 

Instance Method

# ReportLinkStatus

Reports the status of the link between the device and your driver to the system.

DriverKit

``` source
kern_return_t ReportLinkStatus(IOUserNetworkLinkStatus linkStatus, IOUserNetworkMediaType activeMediaType);
```

## Parameters 

`linkStatus`  

The state of the connection to your device. For a list of possible values, see the constants in IOUserNetworkLinkStatus.

`activeMediaType`  

The media type that your device currently supports. The media type must be one you previously reported using the ReportAvailableMediaTypes method.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Call this method when you want to notify the network about any changes to the link status or active media type for your device.

## See Also

### Reporting the Connection Status

ReportLinkQuality

Reports the quality of the link between the device and your driver to the system.

ReportDataBandwidths

Reports the input and output bandwidth between the device and your driver to the system.

IOUserNetworkLinkStatus

A type for specifying the state of your device’s connection.

IOUserNetworkLinkQuality

A type for specifying the quality of your device’s connection to the host.

