

- Core Foundation
-  CFSocketRegisterValue(\_:\_:\_:\_:) 

Function

# CFSocketRegisterValue(\_:\_:\_:\_:)

Registers a property-list value with a CFSocket name server.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketRegisterValue(
    _ nameServerSignature: UnsafePointer!,
    _ timeout: CFTimeInterval,
    _ name: CFString!,
    _ value: CFPropertyList!
) -> CFSocketError
```

## Parameters 

`nameServerSignature`  

The socket signature for the name server. If `NULL`, this function contacts the default server, which is assumed to be a local process using TCP/IP to listen on the port number returned from CFSocketGetDefaultNameRegistryPortNumber(). If `nameServerSignature` is incomplete, the missing values are replaced with the default server’s values, if appropriate.

`timeout`  

The time to wait for the server to accept a connection and to reply to the registration request.

`name`  

The name with which to register `value`.

`value`  

The property-list value to register.

## Return Value

An error code indicating success or failure.

## Discussion

To remove a registered value from the name server, use CFSocketUnregister(_:_:_:).

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

func CFSocketSetDefaultNameRegistryPortNumber(UInt16)

Sets the default port number with which to connect to a CFSocket name server.

func CFSocketUnregister(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!) -> CFSocketError

Unregisters a value or socket signature with a CFSocket name server.

