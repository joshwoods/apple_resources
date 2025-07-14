

- Core Foundation
-  CFSocketUnregister(\_:\_:\_:) 

Function

# CFSocketUnregister(\_:\_:\_:)

Unregisters a value or socket signature with a CFSocket name server.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketUnregister(
    _ nameServerSignature: UnsafePointer!,
    _ timeout: CFTimeInterval,
    _ name: CFString!
) -> CFSocketError
```

## Parameters 

`nameServerSignature`  

The socket signature for the name server. If `NULL`, this function contacts the default server, which is assumed to be a local process using TCP/IP to listen on the port number returned from CFSocketGetDefaultNameRegistryPortNumber(). If `nameServerSignature` is incomplete, the missing values are replaced with the default server’s values, if appropriate.

`timeout`  

The time to wait for the server to accept a connection and to reply to the registration request.

`name`  

The name of the property-list value or socket signature to unregister.

## Return Value

An error code indicating success or failure.

## Discussion

The value being unregistered was previously registered with CFSocketRegisterValue(_:_:_:_:) or CFSocketRegisterSocketSignature(_:_:_:_:).

## See Also

### Core Foundation Socket Name Server Utilities Miscellaneous Functions

func CFSocketCopyRegisteredSocketSignature(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!, UnsafeMutablePointer&lt;CFSocketSignature>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!) -> CFSocketError

Returns a socket signature registered with a CFSocket name server.

func CFSocketCopyRegisteredValue(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFPropertyList>?>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!) -> CFSocketError

Returns a value registered with a CFSocket name server.

func CFSocketGetDefaultNameRegistryPortNumber() -> UInt16

Returns the default port number with which to connect to a CFSocket name server.

func CFSocketRegisterSocketSignature(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!, UnsafePointer&lt;CFSocketSignature>!) -> CFSocketError

Registers a socket signature with a CFSocket name server.

func CFSocketRegisterValue(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!, CFPropertyList!) -> CFSocketError

Registers a property-list value with a CFSocket name server.

func CFSocketSetDefaultNameRegistryPortNumber(UInt16)

Sets the default port number with which to connect to a CFSocket name server.

