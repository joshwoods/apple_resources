

- System Configuration
-  SCNetworkConnectionGetStatus(\_:) 

Function

# SCNetworkConnectionGetStatus(\_:)

Returns the status of the specified network connection.

macOS 10.3+

``` source
func SCNetworkConnectionGetStatus(_ connection: SCNetworkConnection) -> SCNetworkConnectionStatus
```

## Parameters 

`connection`  

The network connection.

## Return Value

The status of the network connection. See SCNetworkConnectionStatus for a list of possible values.

## See Also

### Getting Connection-Status Information

func SCNetworkConnectionGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkConnection` instances.

func SCNetworkConnectionCopyUserPreferences(CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> Bool

Provides the default service ID and a dictionary of user options for the specified connection.

func SCNetworkConnectionCopyServiceID(SCNetworkConnection) -> CFString?

Returns the service ID associated with the specified network connection.

func SCNetworkConnectionCopyExtendedStatus(SCNetworkConnection) -> CFDictionary?

Returns the extended status of the connection.

func SCNetworkConnectionCopyStatistics(SCNetworkConnection) -> CFDictionary?

Returns the statistics of the specified connection.

func SCNetworkConnectionCopyUserOptions(SCNetworkConnection) -> CFDictionary?

Gets the user options used to start the specified connection.

