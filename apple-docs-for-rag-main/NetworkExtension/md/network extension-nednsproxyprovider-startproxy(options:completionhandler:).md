

- Network Extension
- NEDNSProxyProvider
-  startProxy(options:completionHandler:) 

Instance Method

# startProxy(options:completionHandler:)

Starts the DNS proxy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

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

A dictionary that you define as part of a device configuration profile. You can also modify the contents of this dictionary from your app using the shared instance of NEDNSProxyManager. The dictionary appears as the providerConfiguration component of the manager’s providerProtocol property.

`completionHandler`  

A block that you must execute when the proxy is fully established, or when the proxy cannot be started due to an error. If the proxy is successfully established, the error parameter should be set to `nil`. Otherwise, the error parameter passed to this block indicates the reason for failure.

## Discussion

Subclasses of NEDNSProxyProvider must override this method to perform any necessary steps to ready the proxy for handling flows of network data.

The framework calls this method when a new proxy instance is created. You indicate that setup is complete by calling the completion handler with a `nil` error parameter, or that setup failed by calling the completion handler with an error instance. You define the error domain and code.

## See Also

### Managing the DNS proxy life cycle

func stopProxy(with: NEProviderStopReason, completionHandler: () -> Void)

Stops the DNS proxy.

func cancelProxyWithError((any Error)?)

Cancels the DNS proxy.

