

- System Configuration
-  SCNetworkConnectionGetTypeID() 

Function

# SCNetworkConnectionGetTypeID()

Returns the type identifier of all `SCNetworkConnection` instances.

macOS 10.3+

``` source
func SCNetworkConnectionGetTypeID() -> CFTypeID
```

## Return Value

The type identifier of all `SCNetworkConnection` instances.

## See Also

### Getting Connection-Status Information

func SCNetworkConnectionCopyUserPreferences(CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> Bool

Provides the default service ID and a dictionary of user options for the specified connection.

func SCNetworkConnectionCopyServiceID(SCNetworkConnection) -> CFString?

Returns the service ID associated with the specified network connection.

func SCNetworkConnectionGetStatus(SCNetworkConnection) -> SCNetworkConnectionStatus

Returns the status of the specified network connection.

func SCNetworkConnectionCopyExtendedStatus(SCNetworkConnection) -> CFDictionary?

Returns the extended status of the connection.

func SCNetworkConnectionCopyStatistics(SCNetworkConnection) -> CFDictionary?

Returns the statistics of the specified connection.

func SCNetworkConnectionCopyUserOptions(SCNetworkConnection) -> CFDictionary?

Gets the user options used to start the specified connection.

