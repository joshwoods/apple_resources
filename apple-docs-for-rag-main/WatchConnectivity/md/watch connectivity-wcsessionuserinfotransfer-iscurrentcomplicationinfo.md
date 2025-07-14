

- Watch Connectivity
- WCSessionUserInfoTransfer
-  isCurrentComplicationInfo 

Instance Property

# isCurrentComplicationInfo

A Boolean indicating whether the data is related to the app’s complication.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var isCurrentComplicationInfo: Bool { get }
```

## Discussion

This property is set to true if you initiated the transfer using the transferCurrentComplicationUserInfo(_:) method of the WCSession object or false otherwise.

## See Also

### Getting the Transfer Information

var userInfo: [String : Any]

The data being transferred.

