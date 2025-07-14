

- Core Foundation
-  CFSocket 

Class

# CFSocket

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFSocket
```

## Overview

A CFSocket is a communications channel implemented with a BSD socket.

For most uses of this API, you will need to include three headers:

```
#import  #include  #include 
```

CFSocket can be created from scratch with CFSocketCreate(_:_:_:_:_:_:_:) and CFSocketCreateWithSocketSignature(_:_:_:_:_:). CFSocket objects can also be created to wrap an existing BSD socket by calling CFSocketCreateWithNative(_:_:_:_:_:). Finally, you can create a CFSocket and connect simultaneously to a remote host by calling CFSocketCreateConnectedToSocketSignature(_:_:_:_:_:_:).

To listen for messages, you need to create a run loop source with CFSocketCreateRunLoopSource(_:_:_:) and add it to a run loop with CFRunLoopAddSource(_:_:_:). You can select the types of socket activities, such as connection attempts or data arrivals, that cause the source to fire and invoke your CFSocket’s callback function. To send data, you store the data in a CFData and call CFSocketSendData(_:_:_:_:).

Unlike Mach and message ports, sockets support communication over a network.

## Topics

### Creating Sockets

func CFSocketCreate(CFAllocator!, Int32, Int32, Int32, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object of a specified protocol and type.

func CFSocketCreateConnectedToSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!, CFTimeInterval) -> CFSocket!

Creates a CFSocket object and opens a connection to a remote socket.

func CFSocketCreateWithNative(CFAllocator!, CFSocketNativeHandle, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object for a pre-existing native socket.

func CFSocketCreateWithSocketSignature(CFAllocator!, UnsafePointer&lt;CFSocketSignature>!, CFOptionFlags, CFSocketCallBack!, UnsafePointer&lt;CFSocketContext>!) -> CFSocket!

Creates a CFSocket object using information from a CFSocketSignature structure.

### Configuring Sockets

func CFSocketCopyAddress(CFSocket!) -> CFData!

Returns the local address of a CFSocket object.

func CFSocketCopyPeerAddress(CFSocket!) -> CFData!

Returns the remote address to which a CFSocket object is connected.

func CFSocketDisableCallBacks(CFSocket!, CFOptionFlags)

Disables the callback function of a CFSocket object for certain types of socket activity.

func CFSocketEnableCallBacks(CFSocket!, CFOptionFlags)

Enables the callback function of a CFSocket object for certain types of socket activity.

func CFSocketGetContext(CFSocket!, UnsafeMutablePointer&lt;CFSocketContext>!)

Returns the context information for a CFSocket object.

func CFSocketGetNative(CFSocket!) -> CFSocketNativeHandle

Returns the native socket associated with a CFSocket object.

func CFSocketGetSocketFlags(CFSocket!) -> CFOptionFlags

Returns flags that control certain behaviors of a CFSocket object.

func CFSocketSetAddress(CFSocket!, CFData!) -> CFSocketError

Binds a local address to a CFSocket object and configures it for listening.

func CFSocketSetSocketFlags(CFSocket!, CFOptionFlags)

Sets flags that control certain behaviors of a CFSocket object.

### Using Sockets

func CFSocketConnectToAddress(CFSocket!, CFData!, CFTimeInterval) -> CFSocketError

Opens a connection to a remote socket.

func CFSocketCreateRunLoopSource(CFAllocator!, CFSocket!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFSocket object.

func CFSocketGetTypeID() -> CFTypeID

Returns the type identifier for the CFSocket opaque type.

func CFSocketInvalidate(CFSocket!)

Invalidates a CFSocket object, stopping it from sending or receiving any more messages.

func CFSocketIsValid(CFSocket!) -> Bool

Returns a Boolean value that indicates whether a CFSocket object is valid and able to send or receive messages.

func CFSocketSendData(CFSocket!, CFData!, CFData!, CFTimeInterval) -> CFSocketError

Sends data over a CFSocket object.

### Callbacks

typealias CFSocketCallBack

Callback invoked when certain types of activity takes place on a CFSocket object.

### Data Types

struct CFSocketContext

A structure that contains program-defined data and callbacks with which you can configure a CFSocket object’s behavior.

typealias CFSocketNativeHandle

Type for the platform-specific native socket handle.

struct CFSocketSignature

A structure that fully specifies the communication protocol and connection address of a CFSocket object.

### Constants

struct CFSocketCallBackType

Types of socket activity that can cause the callback function of a CFSocket object to be called.

CFSocket Flags

Flags that can be set on a CFSocket object to control its behavior.

enum CFSocketError

Error codes for many CFSocket functions.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Threading Programming Guide

CFNetwork Programming Guide

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

