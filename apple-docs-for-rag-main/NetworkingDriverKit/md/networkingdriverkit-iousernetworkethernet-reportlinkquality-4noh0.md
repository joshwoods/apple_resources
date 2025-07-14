

- NetworkingDriverKit
- IOUserNetworkEthernet
-  ReportLinkQuality 

Instance Method

# ReportLinkQuality

Reports the quality of the link between the device and your driver to the system.

DriverKit

``` source
IOReturn ReportLinkQuality(IOUserNetworkLinkQuality linkQuality);
```

## Parameters 

`linkQuality`  

The quality of the link between your driver and the device. For a list of possible values, see the constants in IOUserNetworkLinkQuality.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Call this method to make the system aware of changes in the quality of the link between your driver and the device.

## See Also

### Reporting the Connection Status

ReportLinkStatus

Reports the status of the link between the device and your driver to the system.

ReportDataBandwidths

Reports the input and output bandwidth between the device and your driver to the system.

IOUserNetworkLinkStatus

A type for specifying the state of your device’s connection.

IOUserNetworkLinkQuality

A type for specifying the quality of your device’s connection to the host.

