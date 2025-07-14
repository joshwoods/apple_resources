

- Network Extension
- NEAppPushProvider
-  start(completionHandler:) 

Instance Method

# start(completionHandler:)

Indicates that the framework has started the provider, and provides a completion handler for subclasses to signal their readiness.

iOS 14.0–18.4DeprecatediPadOS 14.0–18.4DeprecatedMac Catalyst 14.0+visionOS 1.0+

``` source
func start(completionHandler: @escaping ((any Error)?) -> Void)
```

## Parameters 

`completionHandler`  

A Swift closure or ObjectiveC block for your provider subclass to call after it begins connecting to the server. If you can’t connect, pass a non-nil `error` that describes the error, otherwise pass `nil`.

## Mentioned in 

Maintaining a Reliable Network Connection

## Discussion

An NEAppPushProvider subclass must override this method to create a connection with its server.

## See Also

### Implementing provider life cycle

func start()

Indicates that the framework has started the provider.

func stop(with: NEProviderStopReason, completionHandler: () -> Void)

Indicates that the framework needs to stop the provider.

func handleTimerEvent()

Indicates a periodic status check from the framework to the provider.

