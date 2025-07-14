

- Core Foundation
-  CFMessagePort 

Class

# CFMessagePort

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMessagePort
```

## Overview

CFMessagePort objects provide a communications channel that can transmit arbitrary data between multiple threads or processes on the local machine.

You create a local message port with CFMessagePortCreateLocal(_:_:_:_:_:) and make it available to other processes by giving it a name, either when you create it or later with CFMessagePortSetName(_:_:). Other processes then connect to it using CFMessagePortCreateRemote(_:_:), specifying the name of the port.

To listen for messages, you need to create a run loop source with CFMessagePortCreateRunLoopSource(_:_:_:) and add it to a run loop with CFRunLoopAddSource(_:_:_:).

Important

If you want to tear down the connection, you must invalidate the port (using CFMessagePortInvalidate(_:)) before releasing the runloop source and the message port object.

Your message port’s callback function will be called when a message arrives. To send data, you store the data in a CFData object and call CFMessagePortSendRequest(_:_:_:_:_:_:_:). You can optionally have the function wait for a reply and return the reply in another CFData object.

Message ports only support communication on the local machine. For network communication, you have to use a CFSocket object.

## Topics

### Creating a CFMessagePort Object

func CFMessagePortCreateLocal(CFAllocator!, CFString!, CFMessagePortCallBack!, UnsafeMutablePointer&lt;CFMessagePortContext>!, UnsafeMutablePointer&lt;DarwinBoolean>!) -> CFMessagePort!

Returns a local CFMessagePort object.

func CFMessagePortCreateRemote(CFAllocator!, CFString!) -> CFMessagePort!

Returns a CFMessagePort object connected to a remote port.

### Configuring a CFMessagePort Object

func CFMessagePortCreateRunLoopSource(CFAllocator!, CFMessagePort!, CFIndex) -> CFRunLoopSource!

Creates a CFRunLoopSource object for a CFMessagePort object.

func CFMessagePortSetInvalidationCallBack(CFMessagePort!, CFMessagePortInvalidationCallBack!)

Sets the callback function invoked when a CFMessagePort object is invalidated.

func CFMessagePortSetName(CFMessagePort!, CFString!) -> Bool

Sets the name of a local CFMessagePort object.

### Using a Message Port

func CFMessagePortInvalidate(CFMessagePort!)

Invalidates a CFMessagePort object, stopping it from receiving or sending any more messages.

func CFMessagePortSendRequest(CFMessagePort!, Int32, CFData!, CFTimeInterval, CFTimeInterval, CFString!, UnsafeMutablePointer&lt;Unmanaged&lt;CFData>?>!) -> Int32

Sends a message to a remote CFMessagePort object.

func CFMessagePortSetDispatchQueue(CFMessagePort!, dispatch_queue_t!)

Schedules callbacks for the specified message port on the specified dispatch queue.

### Examining a Message Port

func CFMessagePortGetContext(CFMessagePort!, UnsafeMutablePointer&lt;CFMessagePortContext>!)

Returns the context information for a CFMessagePort object.

func CFMessagePortGetInvalidationCallBack(CFMessagePort!) -> CFMessagePortInvalidationCallBack!

Returns the invalidation callback function for a CFMessagePort object.

func CFMessagePortGetName(CFMessagePort!) -> CFString!

Returns the name with which a CFMessagePort object is registered.

func CFMessagePortIsRemote(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object represents a remote port.

func CFMessagePortIsValid(CFMessagePort!) -> Bool

Returns a Boolean value that indicates whether a CFMessagePort object is valid and able to send or receive messages.

### Getting the CFMessagePort Type ID

func CFMessagePortGetTypeID() -> CFTypeID

Returns the type identifier for the CFMessagePort opaque type.

### Callbacks

typealias CFMessagePortCallBack

Callback invoked to process a message received on a CFMessagePort object.

typealias CFMessagePortInvalidationCallBack

Callback invoked when a CFMessagePort object is invalidated.

### Data Types

struct CFMessagePortContext

A structure that contains program-defined data and callbacks with which you can configure a CFMessagePort object’s behavior.

### Constants

CFMessagePortSendRequest Error Codes

Error codes for `CFMessagePortSendRequest`.

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

