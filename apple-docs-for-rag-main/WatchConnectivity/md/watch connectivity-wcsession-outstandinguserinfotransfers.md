

- Watch Connectivity
- WCSession
-  outstandingUserInfoTransfers 

Instance Property

# outstandingUserInfoTransfers

An array of in-progress data transfers.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
var outstandingUserInfoTransfers: [WCSessionUserInfoTransfer] { get }
```

## Discussion

This property contains the WCSessionUserInfoTransfer objects representing the data that you queued using the transferUserInfo(_:) or transferCurrentComplicationUserInfo(_:) methods. Use the objects in this array to cancel specific data transfers.

## See Also

### Transferring Data in the Background

func transferUserInfo([String : Any]) -> WCSessionUserInfoTransfer

Sends the specified data dictionary to the counterpart.

