

- Network Extension
- NEFilterProvider
-  stopFilter(with:completionHandler:) 

Instance Method

# stopFilter(with:completionHandler:)

Stop the filter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func stopFilter(
    with reason: NEProviderStopReason,
    completionHandler: @escaping () -> Void
)
```

``` source
func stopFilter(with reason: NEProviderStopReason) async
```

## Parameters 

`reason`  

An `NEProviderStopReason` code indicating why the filter is being stopped. For a list of possible codes, see NEProvider.

`completionHandler`  

A block that must be executed when the filter is fully stopped.

## Discussion

This method is called by the system to stop the filter.

`NEFilterProvider` subclasses must override this method.

## See Also

### Managing the filter life cycle

func startFilter(completionHandler: ((any Error)?) -> Void)

Start the filter.

