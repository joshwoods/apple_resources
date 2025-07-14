

- System Configuration
-  SCNetworkConnectionCopyStatistics(\_:) 

Function

# SCNetworkConnectionCopyStatistics(\_:)

Returns the statistics of the specified connection.

macOS 10.3+

``` source
func SCNetworkConnectionCopyStatistics(_ connection: SCNetworkConnection) -> CFDictionary?
```

## Parameters 

`connection`  

The network connection.

## Return Value

The statistics dictionary, or `NULL` if an error occurred (use the SCError() function to retrieve the specific error).

## Discussion

A statistics dictionary contains specific dictionaries with statistics for each subcomponent of the service. For example, a statistics dictionary for PPP contains the following sub-dictionaries, keys, and values:

| Sub-dictionary | Key | Value |
|----|----|----|
| PPP | `BytesIn` | The number of bytes going up into the network stack for any networking protocol without the PPP headers and trailers. |
| PPP | `BytesOut` | The number of bytes coming out of the network stack for any networking protocol without the PPP headers and trailers. |
| PPP | `PacketsIn` | The number of packets going up into the network stack for any networking protocol without the PPP headers and trailers. |
| PPP | `PacketsOut` | The number of packets coming out of the network stack for any networking protocol without the PPP headers and trailers. |
| PPP | `ErrorsIn` | The number of errors going up into the network stack for any networking protocol without the PPP headers and trailers. |
| PPP | `ErrorsOut` | The number of errors coming out of the network stack for any networking protocol without the PPP headers and trailers. |

See Statistics Dictionary Keys for the keys to use in the statistics dictionary.

## See Also

### Getting Connection-Status Information

func SCNetworkConnectionGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkConnection` instances.

func SCNetworkConnectionCopyUserPreferences(CFDictionary?, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>, UnsafeMutablePointer&lt;Unmanaged&lt;CFDictionary>?>) -> Bool

Provides the default service ID and a dictionary of user options for the specified connection.

func SCNetworkConnectionCopyServiceID(SCNetworkConnection) -> CFString?

Returns the service ID associated with the specified network connection.

func SCNetworkConnectionGetStatus(SCNetworkConnection) -> SCNetworkConnectionStatus

Returns the status of the specified network connection.

func SCNetworkConnectionCopyExtendedStatus(SCNetworkConnection) -> CFDictionary?

Returns the extended status of the connection.

func SCNetworkConnectionCopyUserOptions(SCNetworkConnection) -> CFDictionary?

Gets the user options used to start the specified connection.

