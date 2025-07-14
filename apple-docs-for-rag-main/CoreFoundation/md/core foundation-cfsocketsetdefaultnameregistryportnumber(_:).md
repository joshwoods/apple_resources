

- Core Foundation
-  CFSocketSetDefaultNameRegistryPortNumber(\_:) 

Function

# CFSocketSetDefaultNameRegistryPortNumber(\_:)

Sets the default port number with which to connect to a CFSocket name server.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketSetDefaultNameRegistryPortNumber(_ port: UInt16)
```

## Parameters 

`port`  

The port number to use to connect to the CFSocket name server.

## Discussion

If you do not provide a name server signature or leave out the socket address in the signature when calling one of the name registry functions, such as CFSocketRegisterSocketSignature(_:_:_:_:), `port` will be used for the connection.

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

func CFSocketUnregister(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!) -> CFSocketError

Unregisters a value or socket signature with a CFSocket name server.

