

- Watch Connectivity
- WCSession
-  transferUserInfo(\_:) 

Instance Method

# transferUserInfo(\_:)

Sends the specified data dictionary to the counterpart.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+visionOS 1.0+watchOS 2.0+

``` source
func transferUserInfo(_ userInfo: [String : Any] = [:]) -> WCSessionUserInfoTransfer
```

## Parameters 

`userInfo`  

A dictionary of property list values that you want to send. You define the contents of the dictionary that your counterpart supports. This parameter must not be `nil`.

## Return Value

A transfer object that you can use to monitor and cancel the operation.

## Discussion

Call this method when you want to send a dictionary of data to the counterpart and ensure that it’s delivered. Dictionaries sent using this method are queued on the other device and delivered in the order in which they were sent. After a transfer begins, the transfer operation continues even if the app is suspended.

This method can only be called while the session is active (the activationState property is set to WCSessionActivationState.activated). Calling this method for an inactive or deactivated session is a programmer error.

Warning

Always test Watch Connectivity data transfers on paired devices. The Simulator app doesn’t support the transferUserInfo(_:) method.

## See Also

### Transferring Data in the Background

var outstandingUserInfoTransfers: [WCSessionUserInfoTransfer]

An array of in-progress data transfers.

