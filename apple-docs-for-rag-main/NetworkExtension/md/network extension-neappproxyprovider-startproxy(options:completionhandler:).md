

- Network Extension
- NEAppProxyProvider
-  startProxy(options:completionHandler:) 

Instance Method

# startProxy(options:completionHandler:)

Start the network proxy.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func startProxy(
    options: [String : Any]? = nil,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func startProxy(options: [String : Any]? = nil) async throws
```

## Parameters 

`options`  

A dictionary passed by the app that requested that the proxy be started. If the starting app did not specify a dictionary of options then this parameter will be nil. If the proxy was started via Connect On Demand, then this parameter will be nil.

`completionHandler`  

A block that must be executed when the proxy is fully established, or when the proxy cannot be started due to an error. If the proxy was successfully established, then the error parameter must be set to nil. If an error occurred, the error parameter passed to this block must be set to a non-nil NSError object.

## Discussion

This method is called by the system to start the network proxy.

`NEAppProxyProvider` subclasses must override this method.

When the App Proxy Provider executes the `completionHandler` block with a nil error parameter, it signals to the system that it is ready to begin handling network data.

The domain and code of the `NSError` object passed to the `completionHandler` block are defined by the App Proxy Provider.

## See Also

### Managing the app proxy life cycle

func stopProxy(with: NEProviderStopReason, completionHandler: () -> Void)

Stop the network proxy.

func cancelProxyWithError((any Error)?)

Stop the network proxy from the App Proxy Provider.

