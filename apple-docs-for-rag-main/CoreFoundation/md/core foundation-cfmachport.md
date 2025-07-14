

- Core Foundation
-  CFMachPort 

Class

# CFMachPort

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMachPort
```

## Overview

A CFMachPort object is a wrapper for a native Mach port (`mach_port_t`). Mach ports are the native communication channel for the macOS kernel.

CFMachPort does not provide a function to send messages, so you primarily use a CFMachPort object if you need to listen to a Mach port that you obtained by other means. You can get a callback when a message arrives on the port or when the port becomes invalid, such as when the native port dies.

To listen for messages you need to create a run loop source with CFMachPortCreateRunLoopSource(_:_:_:) and add it to a run loop with CFRunLoopAddSource(_:_:_:).

Important

If you want to tear down the connection, you must invalidate the port (using CFMachPortInvalidate(_:)) before releasing the runloop source and the Mach port object.

To send data, you must use the Mach APIs with the native Mach port, which is not described here. Alternatively, you can use a CFMessagePort object, which can send arbitrary data.

Mach ports only support communication on the local machine. For network communication, you have to use a CFSocket object.

## Topics

### Creating a CFMachPort Object

func CFMachPortCreate(CFAllocator!, CFMachPortCallBack!, UnsafeMutablePointer&lt;CFMachPortContext>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFMachPort!

Creates a CFMachPort object with a new Mach port.

func CFMachPortCreateWithPort(CFAllocator!, mach_port_t, CFMachPortCallBack!, UnsafeMutablePointer&lt;CFMachPortContext>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFMachPort!

Creates a CFMachPort object for a pre-existing native Mach port.

### Configuring a CFMachPort Object

func CFMachPortInvalidate(CFMachPort!)

Invalidates a CFMachPort object, stopping it from receiving any more messages.

func CFMachPortCreateRunLoopSource(CFAllocator!, CFMachPort!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFMachPort object.

func CFMachPortSetInvalidationCallBack(CFMachPort!, CFMachPortInvalidationCallBack!)

Sets the callback function invoked when a CFMachPort object is invalidated.

### Examining a CFMachPort Object

func CFMachPortGetContext(CFMachPort!, UnsafeMutablePointer&lt;CFMachPortContext>!)

Returns the context information for a CFMachPort object.

func CFMachPortGetInvalidationCallBack(CFMachPort!) -> CFMachPortInvalidationCallBack!

Returns the invalidation callback function for a CFMachPort object.

func CFMachPortGetPort(CFMachPort!) -> mach_port_t

Returns the native Mach port represented by a CFMachPort object.

func CFMachPortIsValid(CFMachPort!) -> Bool

Returns a Boolean value that indicates whether a CFMachPort object is valid and able to receive messages.

### Getting the CFMachPort Type ID

func CFMachPortGetTypeID() -> CFTypeID

Returns the type identifier for the CFMachPort opaque type.

### Callbacks

typealias CFMachPortCallBack

Callback invoked to process a message received on a CFMachPort object.

typealias CFMachPortInvalidationCallBack

Callback invoked when a CFMachPort object is invalidated.

### Data Types

struct CFMachPortContext

A structure that contains program-defined data and callbacks with which you can configure a CFMachPort object’s behavior.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

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

