

- Network Extension
- NEAppProxyProvider
-  stopProxy(with:completionHandler:) 

Instance Method

# stopProxy(with:completionHandler:)

Stop the network proxy.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func stopProxy(
    with reason: NEProviderStopReason,
    completionHandler: @escaping () -> Void
)
```

``` source
func stopProxy(with reason: NEProviderStopReason) async
```

## Parameters 

`reason`  

A `NEProviderStopReason` code indicating why the proxy is being stopped. For a list of possible codes, see NEProvider.

`completionHandler`  

A block that must be executed when the proxy is fully stopped.

## Discussion

This method is called by the system to stop the network proxy.

`NEAppProxyProvider` subclasses must override this method.

Do not use this method to stop the proxy from the App Proxy Provider. Use `cancelProxyWithError:` instead.

## See Also

### Managing the app proxy life cycle

func startProxy(options: [String : Any]?, completionHandler: ((any Error)?) -> Void)

Start the network proxy.

func cancelProxyWithError((any Error)?)

Stop the network proxy from the App Proxy Provider.

