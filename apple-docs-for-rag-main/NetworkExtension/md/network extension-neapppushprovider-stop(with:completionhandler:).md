

- Network Extension
- NEAppPushProvider
-  stop(with:completionHandler:) 

Instance Method

# stop(with:completionHandler:)

Indicates that the framework needs to stop the provider.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+visionOS 1.0+

``` source
func stop(
    with reason: NEProviderStopReason,
    completionHandler: @escaping () -> Void
)
```

``` source
func stop(with reason: NEProviderStopReason) async
```

## Parameters 

`reason`  

An NEProviderStopReason that indicates why the provider needs to stop.

`completionHandler`  

A block that your provider subclass calls after it completely stops.

## Mentioned in 

Maintaining a Reliable Network Connection

## Discussion

An NEAppPushProvider subclass must override this method to perform any necessary tasks when stopping communication with the server.

## See Also

### Implementing provider life cycle

func start()

Indicates that the framework has started the provider.

func start(completionHandler: ((any Error)?) -> Void)

Indicates that the framework has started the provider, and provides a completion handler for subclasses to signal their readiness.

func handleTimerEvent()

Indicates a periodic status check from the framework to the provider.

