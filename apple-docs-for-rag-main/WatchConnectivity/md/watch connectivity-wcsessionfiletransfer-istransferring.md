

- Watch Connectivity
- WCSessionFileTransfer
-  isTransferring 

Instance Property

# isTransferring

A Boolean value indicating whether the file is still being transferred.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var isTransferring: Bool { get }
```

## Discussion

The value of this property is true if the file transfer is not yet complete or false if the transfer is complete.

## See Also

### Managing the File Transfer

var progress: Progress

An object that tracks the progress of the file transfer.

func cancel()

Cancels the file transfer.

