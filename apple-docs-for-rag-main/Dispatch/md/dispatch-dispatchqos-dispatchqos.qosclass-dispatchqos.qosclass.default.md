

- Dispatch
- DispatchQoS
- DispatchQoS.QoSClass
-  DispatchQoS.QoSClass.default 

Case

# DispatchQoS.QoSClass.default

The default quality-of-service class.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
case `default`
```

## Discussion

Default tasks have a lower priority than user-initiated and user-interactive tasks, but a higher priority than utility and background tasks. Assign this class to tasks or queues that your app initiates or uses to perform active work on the user’s behalf.

## See Also

### Getting the Quality-of-Service Class

case userInteractive

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updating your app’s user interface.

case userInitiated

The quality-of-service class for tasks that prevent the user from actively using your app.

case utility

The quality-of-service class for tasks that the user does not track actively.

case background

The quality-of-service class for maintenance or cleanup tasks that you create.

case unspecified

The absence of a quality-of-service class.

