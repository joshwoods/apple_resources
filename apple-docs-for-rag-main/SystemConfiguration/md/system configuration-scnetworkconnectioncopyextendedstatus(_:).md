

- System Configuration
-  SCNetworkConnectionCopyExtendedStatus(\_:) 

Function

# SCNetworkConnectionCopyExtendedStatus(\_:)

Returns the extended status of the connection.

macOS 10.3+

``` source
func SCNetworkConnectionCopyExtendedStatus(_ connection: SCNetworkConnection) -> CFDictionary?
```

## Parameters 

`connection`  

The network connection.

## Return Value

The status dictionary, or `NULL` if an error occurred (use the SCError() function to retrieve the specific error).

## Discussion

An extended status dictionary contains specific dictionaries describing the status for each subcomponent of the service. For example, a status dictionary contains the following sub-dictionaries, keys, and values:

| Sub-dictionary | Key | Value |
|----|----|----|
| IPv4 | `Addresses` | The assigned IP address |
| PPP | `Status` | The PPP-specific status (see SCNetworkConnectionPPPStatus for possible values) |
|  | `LastCause` | Available when the status is “Disconnected” and contains the last error associated with connecting or disconnecting. |
|  | `ConnectTime` | The time when the connection was established. |
| Modem | `ConnectSpeed` | The speed of the modem connection in bits per second. |

Other dictionaries can be present for PPoE, PPTP, and L2TP.

The status dictionary may be extended in the future to contain additional information.

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

func SCNetworkConnectionCopyStatistics(SCNetworkConnection) -> CFDictionary?

Returns the statistics of the specified connection.

func SCNetworkConnectionCopyUserOptions(SCNetworkConnection) -> CFDictionary?

Gets the user options used to start the specified connection.

