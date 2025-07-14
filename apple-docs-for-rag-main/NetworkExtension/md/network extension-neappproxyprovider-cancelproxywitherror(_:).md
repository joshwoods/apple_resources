

- Network Extension
- NEAppProxyProvider
-  cancelProxyWithError(\_:) 

Instance Method

# cancelProxyWithError(\_:)

Stop the network proxy from the App Proxy Provider.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
func cancelProxyWithError(_ error: (any Error)?)
```

## Parameters 

`error`  

An NSError object containing the error that caused the proxy to be stopped. The domain and code of this `NSError` object is defined by the caller.

## Discussion

The App Proxy Provider should call this method when an unrecoverable error occurs that makes the proxy no longer viable.

## See Also

### Managing the app proxy life cycle

func startProxy(options: [String : Any]?, completionHandler: ((any Error)?) -> Void)

Start the network proxy.

func stopProxy(with: NEProviderStopReason, completionHandler: () -> Void)

Stop the network proxy.

