

- NetworkingDriverKit
-  IOUserNetworkMediaType 

Type Alias

# IOUserNetworkMediaType

A structure describing a specific Ethernet type and configuration that your driver supports.

DriverKit

``` source
typedef uint32_t IOUserNetworkMediaType;
```

## Discussion

To specify a media type, combine a media type constant with zero or more configuration options. For example, if your driver supports 10-BaseT Ethernet in full duplex mode, use the following code to configure that media type.

```
```

## Topics

### Configuring the Media Type Information

Media Type Constants

The types of networking media your driver supports.

Configuration Options

The configuration options that you support for a specific network media type.

## See Also

### Declaring the Supported Media Types

ReportAvailableMediaTypes

Tells the system what types of networking media your driver supports.

SelectMediaType

Selects the media type to use when communicating with the network stack.

