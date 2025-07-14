

- Dispatch
- DispatchQoS
- DispatchQoS.QoSClass
-  DispatchQoS.QoSClass.userInteractive 

Case

# DispatchQoS.QoSClass.userInteractive

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updating your app’s user interface.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
case userInteractive
```

## Discussion

User-interactive tasks have the highest priority on the system. Use this class for tasks or queues that interact with the user or actively update your app’s user interface. For example, use this for class for animations or for tracking events interactively.

## See Also

### Getting the Quality-of-Service Class

case userInitiated

The quality-of-service class for tasks that prevent the user from actively using your app.

case `default`

The default quality-of-service class.

case utility

The quality-of-service class for tasks that the user does not track actively.

case background

The quality-of-service class for maintenance or cleanup tasks that you create.

case unspecified

The absence of a quality-of-service class.

