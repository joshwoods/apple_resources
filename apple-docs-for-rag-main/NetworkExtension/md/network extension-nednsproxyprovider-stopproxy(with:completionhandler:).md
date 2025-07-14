

- Network Extension
- NEDNSProxyProvider
-  stopProxy(with:completionHandler:) 

Instance Method

# stopProxy(with:completionHandler:)

Stops the DNS proxy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

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

A code indicating why the proxy is being stopped.

`completionHandler`  

A block that must be called when the proxy is completely stopped.

## Discussion

Subclasses of NEDNSProxyProvider must override this method to perform whatever steps are necessary to stop the proxy.

The system calls this method to stop the proxy. You indicate that the proxy is fully stopped by calling the completion handler.

Important

Don’t call this method to stop the proxy from within the proxy provider itself. Call cancelProxyWithError(_:) instead.

## See Also

### Managing the DNS proxy life cycle

func startProxy(options: [String : Any]?, completionHandler: ((any Error)?) -> Void)

Starts the DNS proxy.

func cancelProxyWithError((any Error)?)

Cancels the DNS proxy.

