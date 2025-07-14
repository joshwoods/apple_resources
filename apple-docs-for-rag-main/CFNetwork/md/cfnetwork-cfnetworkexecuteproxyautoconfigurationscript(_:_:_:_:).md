

- CFNetwork
-  CFNetworkExecuteProxyAutoConfigurationScript(\_:\_:\_:\_:) 

Function

# CFNetworkExecuteProxyAutoConfigurationScript(\_:\_:\_:\_:)

Downloads a proxy autoconfiguration script and executes it.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func CFNetworkExecuteProxyAutoConfigurationScript(
    _ proxyAutoConfigurationScript: CFString,
    _ targetURL: CFURL,
    _ cb: CFProxyAutoConfigurationResultCallback,
    _ clientContext: UnsafeMutablePointer
) -> CFRunLoopSource
```

## Parameters 

`proxyAutoConfigurationScript`  

A `CFString` containing the code of the autoconfiguration script to be executed.

`targetURL`  

The URL that your application intends to eventually download using the proxies.

`cb`  

A callback to be called when execution of the script is finished.

`clientContext`  

A stream context containing a client info object and optionally retain and release callbacks for that object.

## Discussion

This function returns a run loop source that the caller should schedule. Once execution of the script has completed, the specified callback function is called.

Note

If you want to terminate the request before completion, you should invalidate the run loop source.

## See Also

### Global Proxy Configuration

func CFNetworkCopyProxiesForURL(CFURL, CFDictionary) -> Unmanaged&lt;CFArray>

Returns the list of proxies that should be used to download a given URL.

func CFNetworkCopyProxiesForAutoConfigurationScript(CFString, CFURL, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> Unmanaged&lt;CFArray>?

Executes a proxy autoconfiguration script to determine the best proxy to use to retrieve a specified URL.

func CFNetworkExecuteProxyAutoConfigurationURL(CFURL, CFURL, CFProxyAutoConfigurationResultCallback, UnsafeMutablePointer&lt;CFStreamClientContext>) -> CFRunLoopSource

Downloads a proxy autoconfiguration script and executes it.

func CFNetworkCopySystemProxySettings() -> Unmanaged&lt;CFDictionary>?

Returns a CFDictionary containing the current systemwide internet proxy settings.

typealias CFProxyAutoConfigurationResultCallback

Callback function called when a proxy autoconfiguration computation has completed.

Property Keys

Keys for calls to property get/set functions such as CFReadStreamSetProperty(_:_:_:) and CFReadStreamCopyProperty(_:_:).

Proxy Types

Constants that specify the type of proxy.

Global Proxy Settings Constants

Constants for keys in the global proxy settings dictionary returned by CFNetworkCopySystemProxySettings().

