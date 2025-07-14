

- Dispatch
- DispatchQoS
- DispatchQoS.QoSClass
-  DispatchQoS.QoSClass.background 

Case

# DispatchQoS.QoSClass.background

The quality-of-service class for maintenance or cleanup tasks that you create.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
case background
```

## Discussion

Background tasks have the lowest priority of all tasks. Assign this class to tasks or dispatch queues that you use to perform work while your app is running in the background.

## See Also

### Getting the Quality-of-Service Class

case userInteractive

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updating your app’s user interface.

case userInitiated

The quality-of-service class for tasks that prevent the user from actively using your app.

case `default`

The default quality-of-service class.

case utility

The quality-of-service class for tasks that the user does not track actively.

case unspecified

The absence of a quality-of-service class.

