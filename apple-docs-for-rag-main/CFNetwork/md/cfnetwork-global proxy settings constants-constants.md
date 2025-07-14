

- CFNetwork
-  Global Proxy Settings Constants 

API Collection

# Global Proxy Settings Constants

Constants for keys in the global proxy settings dictionary returned by CFNetworkCopySystemProxySettings().

## Topics

### Constants

let kCFNetworkProxiesExceptionsList: CFString

Value is a `CFArray` of `CFString` objects indicating host name patterns that should bypass the proxy.

let kCFNetworkProxiesExcludeSimpleHostnames: CFString

Value is a `CFNumber` object indicating whether simple host names are excluded. Simple host names are excluded if the key is present and the associated value is nonzero.

let kCFNetworkProxiesFTPEnable: CFString

Value is a `CFNumber` object indicating whether an FTP proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesFTPPassive: CFString

Value is a `CFNumber` object indicating whether an FTP proxy’s passive mode is enabled. The passive mode is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesFTPPort: CFString

Value is a `CFNumber` object indicating the port number of an FTP proxy.

let kCFNetworkProxiesFTPProxy: CFString

Value is a `CFString` object indicating the host name or IP number of an FTP proxy.

let kCFNetworkProxiesGopherEnable: CFString

Value is a `CFNumber` object indicating whether a gopher proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesGopherPort: CFString

Value is a `CFNumber` indicating the port number of a gopher proxy.

let kCFNetworkProxiesGopherProxy: CFString

Value is a `CFString` object indicating the host name or IP number of a gopher proxy.

let kCFNetworkProxiesHTTPEnable: CFString

Value is a `CFNumber` object indicating whether an HTTP proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesHTTPPort: CFString

Value is a `CFNumber` object containing the port number associated with the HTTP proxy.

let kCFNetworkProxiesHTTPProxy: CFString

Value is a `CFString` object containing the HTTP proxy host name or IP number.

let kCFNetworkProxiesHTTPSEnable: CFString

Value is a `CFNumber` object indicating whether an HTTPS proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesHTTPSPort: CFString

Value is a `CFNumber` object containing the port number associated with the HTTPS proxy.

let kCFNetworkProxiesHTTPSProxy: CFString

Value is a `CFString` object containing the HTTPS proxy host name or IP number.

let kCFNetworkProxiesRTSPEnable: CFString

Value is a `CFNumber` object indicating whether an RTSP proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesRTSPPort: CFString

Value is a `CFNumber` object containing the port number associated with the RTSP proxy.

let kCFNetworkProxiesRTSPProxy: CFString

Value is a `CFString` object containing the RTSP proxy host name or IP number.

let kCFNetworkProxiesSOCKSEnable: CFString

Value is a `CFNumber` object indicating whether a SOCKS proxy is enabled. The proxy is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesSOCKSPort: CFString

Value is a `CFNumber` object containing the port number associated with the SOCKS proxy.

let kCFNetworkProxiesSOCKSProxy: CFString

Value is a `CFString` object containing the SOCKS proxy host name or IP number.

let kCFNetworkProxiesProxyAutoConfigEnable: CFString

Value is a `CFNumber` object indicating whether proxy autoconfiguration is enabled. Proxy autoconfiguration is enabled if the key is present and the associated value is nonzero.

let kCFNetworkProxiesProxyAutoConfigJavaScript: CFString

Value is a `CFString` object that contains the full JavaScript source of the ProxyAutoConfig (PAC) file.

let kCFNetworkProxiesProxyAutoConfigURLString: CFString

Value is a `CFString` object that contains the URL of the proxy autoconfiguration (PAC) file.

let kCFNetworkProxiesProxyAutoDiscoveryEnable: CFString

Value is a `CFNumber` object indicating whether proxy autodiscovery is enabled. Proxy autodiscovery is enabled if the key is present and the associated value is nonzero.

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

Property Keys

Keys for calls to property get/set functions such as CFReadStreamSetProperty(_:_:_:) and CFReadStreamCopyProperty(_:_:).

Proxy Types

Constants that specify the type of proxy.

