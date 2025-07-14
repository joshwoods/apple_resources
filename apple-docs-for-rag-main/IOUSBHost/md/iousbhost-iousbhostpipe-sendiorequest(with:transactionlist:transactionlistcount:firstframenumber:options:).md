

- IOUSBHost
- IOUSBHostPipe
-  sendIORequest(with:transactionList:transactionListCount:firstFrameNumber:options:) 

Instance Method

# sendIORequest(with:transactionList:transactionListCount:firstFrameNumber:options:)

Mac Catalyst 14.0+macOS 12.0+

``` source
func sendIORequest(
    with data: NSMutableData,
    transactionList: UnsafeMutablePointer,
    transactionListCount: Int,
    firstFrameNumber: UInt64,
    options: IOUSBHostIsochronousTransferOptions = []
) throws
```

## See Also

### Instance Methods

func enqueueIORequest(with: NSMutableData, transactionList: UnsafeMutablePointer&lt;IOUSBHostIsochronousTransaction>, transactionListCount: Int, firstFrameNumber: UInt64, options: IOUSBHostIsochronousTransferOptions, completionHandler: IOUSBHostIsochronousTransactionCompletionHandler?) throws

