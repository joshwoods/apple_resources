

- Core Foundation
- CFRunLoopSourceContext1
-  perform 

Instance Property

# perform

A perform callback for the run loop source. This callback is called when the source has fired.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var perform: ((UnsafeMutableRawPointer?, CFIndex, CFAllocator?, UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!
```

## Parameters 

`msg`  

The Mach message received on the Mach port. The pointer is to a `mach_msg_header_t` structure. A version 0 format trailer (`mach_msg_format_0_trailer_t`) is at the end of the Mach message.

`size`  

Size of the Mach message in `msg`, excluding the message trailer.

`allocator`  

The allocator object that should be used to allocate a reply message.

`info`  

The `info` member of the CFRunLoopSourceContext1 structure that was used when creating the run loop source.

## Return Value

An optional Mach message to be sent in response to the received message. The message must be allocated using `allocator`. Return `NULL` if you want an empty reply returned to the sender.

## Discussion

You only need to provide this callback if you create your own version 1 run loop source. CFMachPort and CFMessagePort run loop sources already implement this callback to forward the received message to the CFMachPort’s or CFMessagePort’s own callback function, which you do need to implement.

