

- USBDriverKit
-  IOUSBAbortOptions 

Enumeration

# IOUSBAbortOptions

Options to use when aborting an I/O request.

DriverKit 19.0+

``` source
enum IOUSBAbortOptions : unsigned int;
```

## Topics

### Getting the Options

kIOUSBAbortAsynchronous

Enqueue the abort request and return immediately.

kIOUSBAbortSynchronous

Enqueue the abort request and wait for it to finish.

## See Also

### Aborting I/O Requests

Abort

Aborts all of the pipe’s pending I/O requests.

