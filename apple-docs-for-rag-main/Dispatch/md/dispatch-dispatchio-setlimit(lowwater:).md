

- Dispatch
- DispatchIO
-  setLimit(lowWater:) 

Instance Method

# setLimit(lowWater:)

Sets the minimum number of bytes to process before enqueueing a handler block.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setLimit(lowWater low_water: Int)
```

## Parameters 

`low_water`  

The minimum number of bytes to read or write before enqueueing the corresponding I/O handler block.

## Discussion

During a read or write operation, the channel uses the high- and low-water mark values to determine how often to enqueue the associated handler block. It enqueues the block when the number of bytes read or written is between these two values. The only times when the number of bytes may be less than the low-water mark are when an EOF is reached or the channel interval has the DISPATCH_IO_STRICT_INTERVAL flag set.

In practice, your handlers should be designed to handle data blocks that are significantly larger than the current low-water mark. If you always want to process the same amount of data in your handler, set the low- and high-water marks to the same value.

The default low-water mark for channels is unspecified. However, you should assume that partial results can be returned even with this default value. If you want to prevent the return of partial results, set the low-water mark to `SIZE_MAX`.

## See Also

### Managing the File Descriptor

var fileDescriptor: Int32

Returns the file descriptor associated with the specified channel.

func setLimit(highWater: Int)

Sets the maximum number of bytes to process before enqueueing a handler block.

func setInterval(interval: DispatchTimeInterval, flags: DispatchIO.IntervalFlags)

Sets the interval, in nanoseconds, at which to invoke the I/O handlers for the channel.

struct IntervalFlags

The desired delivery behavior for interval events.

