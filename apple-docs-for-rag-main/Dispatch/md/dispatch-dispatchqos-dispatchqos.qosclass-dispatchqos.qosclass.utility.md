

- Dispatch
- DispatchQoS
- DispatchQoS.QoSClass
-  DispatchQoS.QoSClass.utility 

Case

# DispatchQoS.QoSClass.utility

The quality-of-service class for tasks that the user does not track actively.

iOS 8.0+iPadOS 8.0+Mac CatalystmacOS 10.10+tvOSvisionOSwatchOS

``` source
case utility
```

## Discussion

Utility tasks have a lower priority than default, user-initiated, and user-interactive tasks, but a higher priority than background tasks. Assign this quality-of-service class to tasks that do not prevent the user from continuing to use your app. For example, you might assign this class to long-running tasks whose progress the user does not follow actively.

## See Also

### Getting the Quality-of-Service Class

case userInteractive

The quality-of-service class for user-interactive tasks, such as animations, event handling, or updating your app’s user interface.

case userInitiated

The quality-of-service class for tasks that prevent the user from actively using your app.

case `default`

The default quality-of-service class.

case background

The quality-of-service class for maintenance or cleanup tasks that you create.

case unspecified

The absence of a quality-of-service class.

