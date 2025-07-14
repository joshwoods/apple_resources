

- Network Extension
- NEDNSProxyProvider
-  cancelProxyWithError(\_:) 

Instance Method

# cancelProxyWithError(\_:)

Cancels the DNS proxy.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func cancelProxyWithError(_ error: (any Error)?)
```

## Parameters 

`error`  

An error instance containing details about the problem that the proxy provider implementation encountered.

## Discussion

Call this method from within the proxy provider when you need to stop the proxy due to a network error that renders the proxy no longer viable.

Important

Subclasses should not override this method.

## See Also

### Managing the DNS proxy life cycle

func startProxy(options: [String : Any]?, completionHandler: ((any Error)?) -> Void)

Starts the DNS proxy.

func stopProxy(with: NEProviderStopReason, completionHandler: () -> Void)

Stops the DNS proxy.

