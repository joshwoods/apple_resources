

- CFNetwork
-  CFProxyAutoConfigurationResultCallback 

Type Alias

# CFProxyAutoConfigurationResultCallback

Callback function called when a proxy autoconfiguration computation has completed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
typealias CFProxyAutoConfigurationResultCallback = (UnsafeMutableRawPointer, CFArray, CFError?) -> Void
```

## Parameters 

`client`  

The client reference originally passed in the `clientContext` parameter of the `CFNetworkExecuteProxyAutoConfigurationScript` or `CFNetworkExecuteProxyAutoConfigurationURL` call that triggered this callback.

`proxyList`  

The list of proxies returned by the autoconfiguration script. This list is in a format suitable for passing to `CFProxyCopyProxiesForURL` (with the added guarantee that no entries will ever be autoconfiguration URL entries). If an error occurs, this value will be `NULL`.

Note

If you want to keep this list, you must retain it when your callback receives it.

`error`  

An error object that indicates any error that may have occurred. If no error occurred, this value will be NULL.

## See Also

### Global Proxy Configuration

func CFNetworkCopyProxiesForURL(CFURL, CFDictionary) -> Unmanaged&lt;CFArray>

Returns the list of proxies that should be used to download a given URL.

func CFNetworkCopyProxiesForAutoConfigurationScript(CFString, CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFArray>?

Executes a proxy autoconfiguration script to determine the best proxy to use to retrieve a specified URL.

func CFNetworkExecuteProxyAutoConfigurationScript(CFString, CFURL, CFProxyAutoConfigurationResultCallback, UnsafeMutablePointer&lt;CFStreamClientContext>) -> CFRunLoopSource

Downloads a proxy autoconfiguration script and executes it.

func CFNetworkExecuteProxyAutoConfigurationURL(CFURL, CFURL, CFProxyAutoConfigurationResultCallback, UnsafeMutablePointer&lt;CFStreamClientContext>) -> CFRunLoopSource

Downloads a proxy autoconfiguration script and executes it.

func CFNetworkCopySystemProxySettings() -> Unmanaged&lt;CFDictionary>?

Returns a CFDictionary containing the current systemwide internet proxy settings.

Property Keys

Keys for calls to property get/set functions such as CFReadStreamSetProperty(_:_:_:) and CFReadStreamCopyProperty(_:_:).

Proxy Types

Constants that specify the type of proxy.

Global Proxy Settings Constants

Constants for keys in the global proxy settings dictionary returned by CFNetworkCopySystemProxySettings().

