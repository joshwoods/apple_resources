

- Watch Connectivity
- WCSession
-  hasContentPending 

Instance Property

# hasContentPending

A Boolean value that indicates whether the session has more content to deliver.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+watchOS 3.0+

``` source
var hasContentPending: Bool { get }
```

## Discussion

true if the session has received data in the background but has not yet delivered that data to the session’s delegate. The following methods send data in the background:

- updateApplicationContext(_:)

- transferUserInfo(_:)

- transferCurrentComplicationUserInfo(_:)

- transferFile(_:metadata:)

## See Also

### Transferring Files in the Background

func transferFile(URL, metadata: [String : Any]?) -> WCSessionFileTransfer

Sends the specified file and optional dictionary to the counterpart.

var outstandingFileTransfers: [WCSessionFileTransfer]

An array of in-progress file transfers.

