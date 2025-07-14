

- NetworkingDriverKit
-  IOUserNetworkLinkStatus 

Type Alias

# IOUserNetworkLinkStatus

A type for specifying the state of your device’s connection.

DriverKit

``` source
typedef uint32_t IOUserNetworkLinkStatus;
```

## Topics

### Specifying the Link Status

Link Status Constants

Constants describing the state of the link between the device and your driver.

## See Also

### Reporting the Connection Status

ReportLinkStatus

Reports the status of the link between the device and your driver to the system.

ReportLinkQuality

Reports the quality of the link between the device and your driver to the system.

ReportDataBandwidths

Reports the input and output bandwidth between the device and your driver to the system.

IOUserNetworkLinkQuality

A type for specifying the quality of your device’s connection to the host.

