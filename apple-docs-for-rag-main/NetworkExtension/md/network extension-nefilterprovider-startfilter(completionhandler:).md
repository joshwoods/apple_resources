

- Network Extension
- NEFilterProvider
-  startFilter(completionHandler:) 

Instance Method

# startFilter(completionHandler:)

Start the filter.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func startFilter(completionHandler: @escaping ((any Error)?) -> Void)
```

``` source
func startFilter() async throws
```

## Parameters 

`completionHandler`  

A block that must be executed when the filter is running and is ready to filter network content.

## Discussion

This method is called by the system to start the filter.

`NEFilterProvider` subclasses must override this method.

When this method is called, the Filter Provider should perform any steps necessary to initialize the filter and then execute the `completionHandler` block.

## See Also

### Managing the filter life cycle

func stopFilter(with: NEProviderStopReason, completionHandler: () -> Void)

Stop the filter.

