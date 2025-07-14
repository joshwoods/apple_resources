

- IOUSBHost
- IOUSBHostPipe
-  enqueueIORequest(with:completionTimeout:completionHandler:) 

Instance Method

# enqueueIORequest(with:completionTimeout:completionHandler:)

Enqueues an input/output request on the pipe.

Mac Catalyst 14.0+macOS 10.15+

``` source
func enqueueIORequest(
    with data: NSMutableData?,
    completionTimeout: TimeInterval,
    completionHandler: IOUSBHostCompletionHandler? = nil
) throws
```

``` source
func enqueueIORequest(
    with data: NSMutableData?,
    completionTimeout: TimeInterval
) async throws -> (IOReturn, Int)
```

## Parameters 

`data`  

An NSMutableData object defining the memory to use for the transfer. Use nil to send a zero-length packet.

`completionTimeout`  

A TimeInterval value representing the timeout of the request. If `0`, the request never times out. Use IOUSBHostDefaultControlCompletionTimeout unless there’s a need for a specific timeout.

`completionHandler`  

An IOUSBHostCompletionHandler that runs when the request completes, or times out after the call returns successfully. If the method returns with an error, the completion handler doesn’t run.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Use this method to issue an asynchronous input/output request on a bulk or interrupt pipe.

## See Also

### Sending Bulk and Interrupt I/O

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

let IOUSBHostDefaultControlCompletionTimeout: TimeInterval

The default completion timeout for input/output requests.

func clearStall() throws

Clears the halt condition of the pipe.

