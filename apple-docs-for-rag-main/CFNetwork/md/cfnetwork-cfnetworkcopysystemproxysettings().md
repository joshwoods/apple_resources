

- CFNetwork
-  CFNetworkCopySystemProxySettings() 

Function

# CFNetworkCopySystemProxySettings()

Returns a CFDictionary containing the current systemwide internet proxy settings.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+

``` source
func CFNetworkCopySystemProxySettings() -> Unmanaged?
```

## Discussion

The dictionary returned contains key-value pairs that represent the current internet proxy settings. The keys in this dictionary are defined in Global Proxy Settings Constants.

The caller is responsible for releasing the returned dictionary.

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

typealias CFProxyAutoConfigurationResultCallback

Callback function called when a proxy autoconfiguration computation has completed.

Property Keys

Keys for calls to property get/set functions such as CFReadStreamSetProperty(_:_:_:) and CFReadStreamCopyProperty(_:_:).

Proxy Types

Constants that specify the type of proxy.

Global Proxy Settings Constants

Constants for keys in the global proxy settings dictionary returned by CFNetworkCopySystemProxySettings().

