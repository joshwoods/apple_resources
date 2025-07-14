

- Watch Connectivity
- WCSession
-  transferCurrentComplicationUserInfo(\_:) 

Instance Method

# transferCurrentComplicationUserInfo(\_:)

Sends complication-related data from the iOS app to the WatchKit extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+

``` source
func transferCurrentComplicationUserInfo(_ userInfo: [String : Any] = [:]) -> WCSessionUserInfoTransfer
```

## Parameters 

`userInfo`  

A dictionary of property list values that you want to send. You define the contents of the dictionary that your counterpart supports. This parameter must not be `nil`.

## Return Value

A transfer object that you can use to monitor and cancel the operation.

## Discussion

Call this method when you have new data to send to your complication. Your WatchKit extension can use the data to replace or extend its current timeline entries.

This method can only be called while the session is active (the activationState property is set to WCSessionActivationState.activated). Calling this method for an inactive or deactivated session is a programmer error.

Warning

Always test Watch Connectivity data transfers on paired devices. The Simulator app doesn’t support the transferCurrentComplicationUserInfo(_:) method.

## See Also

### Updating Complication Data

var remainingComplicationUserInfoTransfers: Int

The number of remaining times you can send complication data from the iOS app to the WatchKit extension.

