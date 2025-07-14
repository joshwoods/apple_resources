

- Watch Connectivity
- WCSessionFileTransfer
-  cancel() 

Instance Method

# cancel()

Cancels the file transfer.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
func cancel()
```

## Discussion

Use this method to cancel a file transfer before it completes. If the file has already been transferred, calling this method has no effect.

## See Also

### Managing the File Transfer

var isTransferring: Bool

A Boolean value indicating whether the file is still being transferred.

var progress: Progress

An object that tracks the progress of the file transfer.

