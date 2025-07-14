

- Network Extension
- NEAppPushProvider
-  handleTimerEvent() 

Instance Method

# handleTimerEvent()

Indicates a periodic status check from the framework to the provider.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func handleTimerEvent()
```

## Mentioned in 

Maintaining a Reliable Network Connection

## Discussion

Implement this method to have your extension check its connection to the server, and trigger a reconnect if necessary.

## See Also

### Implementing provider life cycle

func start()

Indicates that the framework has started the provider.

func start(completionHandler: ((any Error)?) -> Void)

Indicates that the framework has started the provider, and provides a completion handler for subclasses to signal their readiness.

func stop(with: NEProviderStopReason, completionHandler: () -> Void)

Indicates that the framework needs to stop the provider.

