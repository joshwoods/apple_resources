

- USBDriverKit
- IOUSBHostPipe
-  Abort 

Instance Method

# Abort

Aborts all of the pipe’s pending I/O requests.

DriverKit 19.0+

``` source
kern_return_t Abort(IOOptionBits options, kern_return_t withError, IOService * forClient);
```

## Parameters 

`options`  

Options for how to abort the requests. For a list of possible values, see IOUSBAbortOptions.

`withError`  

The error value to report for each request. Specify `kIOReturnAborted` for this parameter.

`forClient`  

The service that initiated the requests. Specify a non `NULL` value for this parameter only for pipes associated with a control endpoint; specify `NULL` for other endpoint types. For a control endpoint, you can also specify `NULL` to abort all requests.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

If the `options` argument includes `kAbortSynchronous`, this method blocks all new I/O requests except those submitted by an aborted completion routine.

## See Also

### Aborting I/O Requests

IOUSBAbortOptions

Options to use when aborting an I/O request.

