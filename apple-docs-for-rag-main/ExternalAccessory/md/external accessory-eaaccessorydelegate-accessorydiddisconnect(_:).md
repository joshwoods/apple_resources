

- External Accessory
- EAAccessoryDelegate
-  accessoryDidDisconnect(\_:) 

Instance Method

# accessoryDidDisconnect(\_:)

Tells the delegate that the specified accessory was disconnected from the device.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.13+tvOS 10.0+visionOS 1.0+

``` source
optional func accessoryDidDisconnect(_ accessory: EAAccessory)
```

## Parameters 

`accessory`  

The accessory that was disconnected.

## Discussion

The accessory manager calls this method as a convenience whenever it receives an EAAccessoryDidDisconnectNotification notification. You can use this method to remove any references to the specified accessory object and to stop any services currently using the accessory.

Because this is a convenience method, your delegate does not also need to register as an observer of the EAAccessoryDidDisconnectNotification notification. However, if you want your delegate to be notified of newly connected accessories, you should configure it as an observer of the EAAccessoryDidConnectNotification notification.

