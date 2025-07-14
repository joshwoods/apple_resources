

- IOKit
- IOKitLib.h
-  IOServiceMatchingCallback 

Type Alias

# IOServiceMatchingCallback

Callback function to be notified of IOService publication.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
typealias IOServiceMatchingCallback = (UnsafeMutableRawPointer?, io_iterator_t) -> Void
```

## Parameters 

`refcon`  

The refcon passed when the notification was installed.

`iterator`  

The notification iterator which now has new objects.

## See Also

### Callbacks

typealias IOAsyncCallback

standard callback function for asynchronous I/O requests with lots of extra arguments beyond a refcon and result code.

typealias IOAsyncCallback0

standard callback function for asynchronous I/O requests with no extra arguments beyond a refcon and result code.

typealias IOAsyncCallback1

standard callback function for asynchronous I/O requests with one extra argument beyond a refcon and result code. This is often a count of the number of bytes transferred

typealias IOAsyncCallback2

standard callback function for asynchronous I/O requests with two extra arguments beyond a refcon and result code.

typealias IOServiceInterestCallback

Callback function to be notified of changes in state of an IOService.

