

- Dispatch
- DispatchIO
-  setLimit(highWater:) 

Instance Method

# setLimit(highWater:)

Sets the maximum number of bytes to process before enqueueing a handler block.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setLimit(highWater high_water: Int)
```

## Parameters 

`high_water`  

The maximum number of bytes to read or write before enqueueing the corresponding I/O handler block.

## Discussion

During a read or write operation, the channel uses the high- and low-water mark values to determine how often to enqueue the associated handler block. It enqueues the block when the number of bytes read or written is between these two values.

The default high-water mark for channels is set to `SIZE_MAX`.

## See Also

### Managing the File Descriptor

var fileDescriptor: Int32

Returns the file descriptor associated with the specified channel.

func setLimit(lowWater: Int)

Sets the minimum number of bytes to process before enqueueing a handler block.

func setInterval(interval: DispatchTimeInterval, flags: DispatchIO.IntervalFlags)

Sets the interval, in nanoseconds, at which to invoke the I/O handlers for the channel.

struct IntervalFlags

The desired delivery behavior for interval events.

