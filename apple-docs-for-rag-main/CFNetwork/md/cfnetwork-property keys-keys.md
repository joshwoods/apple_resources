

- CFNetwork
-  Property Keys 

API Collection

# Property Keys

Keys for calls to property get/set functions such as CFReadStreamSetProperty(_:_:_:) and CFReadStreamCopyProperty(_:_:).

## Topics

### Constants

let kCFProxyAutoConfigurationHTTPResponseKey: CFString

let kCFProxyAutoConfigurationJavaScriptKey: CFString

let kCFProxyAutoConfigurationURLKey: CFString

let kCFProxyHostNameKey: CFString

let kCFProxyPasswordKey: CFString

let kCFProxyPortNumberKey: CFString

let kCFProxyTypeKey: CFString

let kCFProxyUsernameKey: CFString

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

typealias CFProxyAutoConfigurationResultCallback

Callback function called when a proxy autoconfiguration computation has completed.

Proxy Types

Constants that specify the type of proxy.

Global Proxy Settings Constants

Constants for keys in the global proxy settings dictionary returned by CFNetworkCopySystemProxySettings().

