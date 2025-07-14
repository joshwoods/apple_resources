

- NetworkingDriverKit
- IOUserNetworkEthernet
-  ReportAvailableMediaTypes 

Instance Method

# ReportAvailableMediaTypes

Tells the system what types of networking media your driver supports.

DriverKit

``` source
kern_return_t ReportAvailableMediaTypes(const IOUserNetworkMediaType * mediaTypes, uint32_t count);
```

## Parameters 

`mediaTypes`  

An array of IOUserNetworkMediaType types. For each type, combine a Media Type Constants constant with one or more Configuration Options constants to indicate the configurations you support.

`count`  

The number of items in the `mediaTypes` array.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## Discussion

Apple recommends that you include kIOUserNetworkMediaEthernetAuto as one of the media types you support. That media type lets the system configure the networking stack automatically on your behalf, based on the other media types you specify.

## See Also

### Declaring the Supported Media Types

SelectMediaType

Selects the media type to use when communicating with the network stack.

IOUserNetworkMediaType

A structure describing a specific Ethernet type and configuration that your driver supports.

