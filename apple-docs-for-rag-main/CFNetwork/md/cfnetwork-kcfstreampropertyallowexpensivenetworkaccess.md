

- CFNetwork
-  kCFStreamPropertyAllowExpensiveNetworkAccess 

Global Variable

# kCFStreamPropertyAllowExpensiveNetworkAccess

A Boolean value that indicates whether connections may use a network interface that the system considers expensive.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
let kCFStreamPropertyAllowExpensiveNetworkAccess: CFString
```

## Discussion

The default value is kCFBooleanTrue and allows the use of expensive network interfaces. Set this property to kCFBooleanFalse to disallow the use of expensive network interfaces. For more information about expensive network interfaces, see allowsExpensiveNetworkAccess.

## See Also

### Constants

let kCFHTTPVersion3_0: CFString

HTTP version 3.0.

let kCFStreamNetworkServiceTypeAVStreaming: CFString

A multimedia audio and video streaming service.

let kCFStreamNetworkServiceTypeResponsiveAV: CFString

A responsive, time-sensitive, multimedia audio and video service.

let kCFStreamNetworkServiceTypeResponsiveData: CFString

A responsive, time-sensitive data service.

let kCFStreamPropertyAllowConstrainedNetworkAccess: CFString

A Boolean value that indicates whether connections may use the network when the user has specified Low Data Mode.

let kCFStreamPropertyConnectionIsExpensive: CFString

A Boolean value that indicates if the connection is using a network interface that the system considers expensive.

