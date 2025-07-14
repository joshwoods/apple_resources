

- IOKit
- IOKitLib.h
-  IOAsyncCallback2 

Type Alias

# IOAsyncCallback2

standard callback function for asynchronous I/O requests with two extra arguments beyond a refcon and result code.

iOS 18.4+iPadOS 18.4+Mac Catalyst 13.0+macOS 10.0+visionOS 2.4+

``` source
typealias IOAsyncCallback2 = (UnsafeMutableRawPointer?, IOReturn, UnsafeMutableRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`refcon`  

The refcon passed into the original I/O request

`result`  

The result of the I/O operation

`arg0`  

Extra argument

`arg1`  

Extra argument

## See Also

### Callbacks

typealias IOAsyncCallback

standard callback function for asynchronous I/O requests with lots of extra arguments beyond a refcon and result code.

typealias IOAsyncCallback0

standard callback function for asynchronous I/O requests with no extra arguments beyond a refcon and result code.

typealias IOAsyncCallback1

standard callback function for asynchronous I/O requests with one extra argument beyond a refcon and result code. This is often a count of the number of bytes transferred

typealias IOServiceInterestCallback

Callback function to be notified of changes in state of an IOService.

typealias IOServiceMatchingCallback

Callback function to be notified of IOService publication.

