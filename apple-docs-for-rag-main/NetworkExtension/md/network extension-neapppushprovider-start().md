

- Network Extension
- NEAppPushProvider
-  start() 

Instance Method

# start()

Indicates that the framework has started the provider.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
func start()
```

## Discussion

An NEAppPushProvider subclass must override this method to create a connection with its server.

## See Also

### Implementing provider life cycle

func start(completionHandler: ((any Error)?) -> Void)

Indicates that the framework has started the provider, and provides a completion handler for subclasses to signal their readiness.

func stop(with: NEProviderStopReason, completionHandler: () -> Void)

Indicates that the framework needs to stop the provider.

func handleTimerEvent()

Indicates a periodic status check from the framework to the provider.

