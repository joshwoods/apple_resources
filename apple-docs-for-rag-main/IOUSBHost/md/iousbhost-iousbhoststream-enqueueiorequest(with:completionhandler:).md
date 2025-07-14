

- IOUSBHost
- IOUSBHostStream
-  enqueueIORequest(with:completionHandler:) 

Instance Method

# enqueueIORequest(with:completionHandler:)

Enqueues an input/output request on the stream.

Mac Catalyst 14.0+macOS 10.15+

``` source
func enqueueIORequest(
    with data: NSMutableData?,
    completionHandler: IOUSBHostCompletionHandler? = nil
) throws
```

``` source
func enqueueIORequest(with data: NSMutableData?) async throws -> (IOReturn, Int)
```

## Parameters 

`data`  

An NSMutableData object defining the memory to use for the transfer.

`completionHandler`  

An IOUSBHostCompletionHandler that runs when the request completes. The `completionHandler` doesn’t run if the method returns an error.

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func enqueueIORequest(with data: NSMutableData?) async throws -> (IOReturn, Int)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

This method sends an asynchronous request on the stream.

Note

Completion timeouts aren’t applicable to streams.

## See Also

### Sending I/O

typealias IOUSBHostCompletionHandler

The completion handler for asynchronous control, bulk, and interrupt transfers.

func abort(with: IOUSBHostAbortOption) throws

Aborts pending input/output requests.

func abort() throws

Aborts pending input/output requests synchronously.

