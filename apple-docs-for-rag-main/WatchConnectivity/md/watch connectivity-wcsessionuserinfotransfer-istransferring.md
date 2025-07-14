

- Watch Connectivity
- WCSessionUserInfoTransfer
-  isTransferring 

Instance Property

# isTransferring

A Boolean value indicating whether the data is still being transferred.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 2.0+

``` source
var isTransferring: Bool { get }
```

## Discussion

The value of this property is true if the data has not yet been transferred or false if the transfer is complete.

## See Also

### Managing the Transfer Operation

func cancel()

Cancels the data transfer.

