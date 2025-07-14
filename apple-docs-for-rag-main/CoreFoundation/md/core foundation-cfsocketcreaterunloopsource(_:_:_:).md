

- Core Foundation
-  CFSocketCreateRunLoopSource(\_:\_:\_:) 

Function

# CFSocketCreateRunLoopSource(\_:\_:\_:)

Creates a CFRunLoopSource object for a CFSocket object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSocketCreateRunLoopSource(
    _ allocator: CFAllocator!,
    _ s: CFSocket!,
    _ order: CFIndex
) -> CFRunLoopSource!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`s`  

The CFSocket object for which to create a run loop source.

`order`  

A priority index indicating the order in which run loop sources are processed. When multiple run loop sources are firing in a single pass through the run loop, the sources are processed in increasing order of this parameter. If the run loop is set to process only one source per loop, only the highest priority source, the one with the lowest `order` value, is processed.

## Return Value

The new CFRunLoopSource object for `s`. Ownership follows the The Create Rule.

## Discussion

The run loop source is not automatically added to a run loop. To add the source to a run loop, use CFRunLoopAddSource(_:_:_:).

## See Also

### Using Sockets

func CFSocketConnectToAddress(CFSocket!, CFData!, CFTimeInterval) -> CFSocketError

Opens a connection to a remote socket.

func CFSocketGetTypeID() -> CFTypeID

Returns the type identifier for the CFSocket opaque type.

func CFSocketInvalidate(CFSocket!)

Invalidates a CFSocket object, stopping it from sending or receiving any more messages.

func CFSocketIsValid(CFSocket!) -> Bool

Returns a Boolean value that indicates whether a CFSocket object is valid and able to send or receive messages.

func CFSocketSendData(CFSocket!, CFData!, CFData!, CFTimeInterval) -> CFSocketError

Sends data over a CFSocket object.

