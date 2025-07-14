

- Core Foundation
-  Socket Name Server Utilities 

API Collection

# Socket Name Server Utilities

## Overview

Name server functionality is currently inoperable in macOS.

## Topics

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

func CFSocketUnregister(UnsafePointer&lt;CFSocketSignature>!, CFTimeInterval, CFString!) -> CFSocketError

Unregisters a value or socket signature with a CFSocket name server.

### Constants

CFSocket Name Server Keys

Not used.

## See Also

### Utilities

Base Utilities

Byte-Order Utilities

Core Foundation URL Access Utilities

Preferences Utilities

Time Utilities

