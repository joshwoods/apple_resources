

- System Configuration
-  SCNetworkConnectionCopyUserPreferences(\_:\_:\_:) 

Function

# SCNetworkConnectionCopyUserPreferences(\_:\_:\_:)

Provides the default service ID and a dictionary of user options for the specified connection.

macOS 10.3+

``` source
func SCNetworkConnectionCopyUserPreferences(
    _ selectionOptions: CFDictionary?,
    _ serviceID: UnsafeMutablePointer?>,
    _ userOptions: UnsafeMutablePointer?>
) -> Bool
```

## Parameters 

`selectionOptions`  

Currently unimplemented. Pass `NULL`.

`serviceID`  

On output, a reference to the default service ID for starting connections.

`userOptions`  

On output, a reference to the default user options dictionary for starting connections.

## Return Value

`TRUE` if there is a valid service to dial; `FALSE` if the function was unable to retrieve a service to dial.

## Discussion

You can use the service ID and user options values returned by this function to open a connection on the fly.

## See Also

### Getting Connection-Status Information

func SCNetworkConnectionGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkConnection` instances.

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

