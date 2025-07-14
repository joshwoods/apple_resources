

- NetworkingDriverKit
- IOUserNetworkEthernet
-  ReportDataBandwidths 

Instance Method

# ReportDataBandwidths

Reports the input and output bandwidth between the device and your driver to the system.

DriverKit

``` source
kern_return_t ReportDataBandwidths(uint64_t maxInputBandwidth, uint64_t maxOutputBandwidth, uint64_t effectiveInputBandwidth, uint64_t effectiveOutputBandwidth);
```

## Parameters 

`maxInputBandwidth`  

The maximum theoretical data rate for receiving data with the current medium, in bits per second.

`maxOutputBandwidth`  

The maximum theoretical data rate for sending data with the current medium, in bits per second.

`effectiveInputBandwidth`  

The effective input bandwidth, in bits per second. If you specify `0`, the system sets the effective bandwidth to the same value in `maxInputBandwidth`.

`effectiveOutputBandwidth`  

The effective output bandwidth, in bits per second. If you specify `0`, the system sets the effective bandwidth to the same value in `maxOutputBandwidth`.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Reporting the Connection Status

ReportLinkStatus

Reports the status of the link between the device and your driver to the system.

ReportLinkQuality

Reports the quality of the link between the device and your driver to the system.

IOUserNetworkLinkStatus

A type for specifying the state of your device’s connection.

IOUserNetworkLinkQuality

A type for specifying the quality of your device’s connection to the host.

