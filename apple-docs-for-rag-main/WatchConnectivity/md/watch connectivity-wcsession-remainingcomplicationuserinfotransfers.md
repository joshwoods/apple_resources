

- Watch Connectivity
- WCSession
-  remainingComplicationUserInfoTransfers 

Instance Property

# remainingComplicationUserInfoTransfers

The number of remaining times you can send complication data from the iOS app to the WatchKit extension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var remainingComplicationUserInfoTransfers: Int { get }
```

## Discussion

The number of remaining times that you can call transferCurrentComplicationUserInfo(_:) during the current day. If this property is set to 0, any additional calls to transferCurrentComplicationUserInfo(_:) use transferUserInfo(_:) instead.

If the complication is on the active watch face, you are given 50 transfers a day. If the complication is not active, this property defaults to 0.

## See Also

### Updating Complication Data

func transferCurrentComplicationUserInfo([String : Any]) -> WCSessionUserInfoTransfer

Sends complication-related data from the iOS app to the WatchKit extension.

