

- Watch Connectivity
- WCSessionUserInfoTransfer
-  cancel() 

Instance Method

# cancel()

Cancels the data transfer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func cancel()
```

## Discussion

Use this method to cancel a transfer before it completes. If the data has already been transferred, calling this method has no effect.

## See Also

### Managing the Transfer Operation

var isTransferring: Bool

A Boolean value indicating whether the data is still being transferred.

