

- Dispatch
- DispatchIO
-  fileDescriptor 

Instance Property

# fileDescriptor

Returns the file descriptor associated with the specified channel.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var fileDescriptor: Int32 { get }
```

## Discussion

If the path name associated with the channel has not yet been opened, calling this function does not normally open the corresponding file, with one exception. If you call the function from a barrier block scheduled on the channel, the function does open the file and return the resulting file descriptor.

## See Also

### Managing the File Descriptor

func setLimit(highWater: Int)

Sets the maximum number of bytes to process before enqueueing a handler block.

func setLimit(lowWater: Int)

Sets the minimum number of bytes to process before enqueueing a handler block.

func setInterval(interval: DispatchTimeInterval, flags: DispatchIO.IntervalFlags)

Sets the interval, in nanoseconds, at which to invoke the I/O handlers for the channel.

struct IntervalFlags

The desired delivery behavior for interval events.

