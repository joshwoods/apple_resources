

- IOKit
- IOKitLib.h
-  IOAsyncCallback 

Type Alias

# IOAsyncCallback

standard callback function for asynchronous I/O requests with lots of extra arguments beyond a refcon and result code.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
typealias IOAsyncCallback = (UnsafeMutableRawPointer?, IOReturn, UnsafeMutablePointer?, UInt32) -> Void
```

## Parameters 

`refcon`  

The refcon passed into the original I/O request

`result`  

The result of the I/O operation

`args`  

Array of extra arguments

`numArgs`  

Number of extra arguments

## See Also

### Callbacks

typealias IOAsyncCallback0

standard callback function for asynchronous I/O requests with no extra arguments beyond a refcon and result code.

typealias IOAsyncCallback1

standard callback function for asynchronous I/O requests with one extra argument beyond a refcon and result code. This is often a count of the number of bytes transferred

typealias IOAsyncCallback2

standard callback function for asynchronous I/O requests with two extra arguments beyond a refcon and result code.

typealias IOServiceInterestCallback

Callback function to be notified of changes in state of an IOService.

typealias IOServiceMatchingCallback

Callback function to be notified of IOService publication.

