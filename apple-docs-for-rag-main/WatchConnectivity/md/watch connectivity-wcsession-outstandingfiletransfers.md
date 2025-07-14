

- Watch Connectivity
- WCSession
-  outstandingFileTransfers 

Instance Property

# outstandingFileTransfers

An array of in-progress file transfers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outstandingFileTransfers: [WCSessionFileTransfer] { get }
```

## Discussion

This property contains the WCSessionFileTransfer objects representing the files that are queued for delivery but have not yet been delivered to the counterpart. You can use the objects to cancel specific file transfers.

## See Also

### Transferring Files in the Background

func transferFile(URL, metadata: [String : Any]?) -> WCSessionFileTransfer

Sends the specified file and optional dictionary to the counterpart.

var hasContentPending: Bool

A Boolean value that indicates whether the session has more content to deliver.

