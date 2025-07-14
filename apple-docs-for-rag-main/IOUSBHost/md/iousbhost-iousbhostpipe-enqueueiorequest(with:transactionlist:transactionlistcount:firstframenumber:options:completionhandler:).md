

- IOUSBHost
- IOUSBHostPipe
-  enqueueIORequest(with:transactionList:transactionListCount:firstFrameNumber:options:completionHandler:) 

Instance Method

# enqueueIORequest(with:transactionList:transactionListCount:firstFrameNumber:options:completionHandler:)

Mac Catalyst 14.0+macOS 12.0+

``` source
func enqueueIORequest(
    with data: NSMutableData,
    transactionList: UnsafeMutablePointer,
    transactionListCount: Int,
    firstFrameNumber: UInt64,
    options: IOUSBHostIsochronousTransferOptions = [],
    completionHandler: IOUSBHostIsochronousTransactionCompletionHandler? = nil
) throws
```

``` source
func enqueueIORequest(
    with data: NSMutableData,
    transactionList: UnsafeMutablePointer,
    transactionListCount: Int,
    firstFrameNumber: UInt64,
    options: IOUSBHostIsochronousTransferOptions = []
) async throws -> (IOReturn, UnsafeMutablePointer)
```

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func enqueueIORequest(with data: NSMutableData, transactionList: UnsafeMutablePointer, transactionListCount: Int, firstFrameNumber: UInt64, options: IOUSBHostIsochronousTransferOptions = []) async throws -> (IOReturn, UnsafeMutablePointer)
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

## See Also

### Instance Methods

func sendIORequest(with: NSMutableData, transactionList: UnsafeMutablePointer&lt;IOUSBHostIsochronousTransaction>, transactionListCount: Int, firstFrameNumber: UInt64, options: IOUSBHostIsochronousTransferOptions) throws

