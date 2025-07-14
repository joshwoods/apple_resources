

- System Configuration
-  SCNetworkConnectionCallBack 

Type Alias

# SCNetworkConnectionCallBack

The type of callback function used when a status event is delivered.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias SCNetworkConnectionCallBack = (SCNetworkConnection, SCNetworkConnectionStatus, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`connection`  

The network connection.

`status`  

The connection status.

`info`  

Application-specific information.

## Topics

### Fields

connection

The network connection.

status

The connection status.

## See Also

### Data Types

class SCNetworkConnection

The handle to manage a connection-oriented service.

struct SCNetworkConnectionContext

A structure containing user-specified data and callbacks for a network connection.

