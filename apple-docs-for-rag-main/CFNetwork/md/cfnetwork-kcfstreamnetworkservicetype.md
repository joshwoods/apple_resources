

- CFNetwork
-  kCFStreamNetworkServiceType 

Global Variable

# kCFStreamNetworkServiceType

The type of service for the stream. Providing the service type allows the system to properly handle certain attributes of the stream, including routing and suspension behavior. Most streams do not need to set this property. See Stream Service Types for a list of possible values.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let kCFStreamNetworkServiceType: CFString
```

## See Also

### Streams

func CFReadStreamCreateForHTTPRequest(CFAllocator?, CFHTTPMessage) -> Unmanaged&lt;CFReadStream>

Creates a read stream for a CFHTTP request message.

Deprecated

func CFReadStreamCreateForStreamedHTTPRequest(CFAllocator?, CFHTTPMessage, CFReadStream) -> Unmanaged&lt;CFReadStream>

Creates a read stream for a CFHTTP request message object whose body is too long to keep in memory.

Deprecated

let kCFStreamPropertyHTTPAttemptPersistentConnection: CFStringDeprecated

let kCFStreamPropertyHTTPFinalRequest: CFString

HTTP Final Request property. A value of type CFHTTPMessage containing the final message transmitted by the stream after all modifications (including authentication, connection policy, redirects, and so on) have been made. This property cannot be set.

Deprecated

let kCFStreamPropertyHTTPFinalURL: CFString

HTTP Final URL property. A value of type CFURL containing the final HTTP URL. This value differs from the URL in the original HTTP request if an autoredirection occurred. This property cannot be set.

Deprecated

let kCFStreamPropertyHTTPProxy: CFStringDeprecated

let kCFStreamPropertyHTTPProxyHost: CFStringDeprecated

let kCFStreamPropertyHTTPProxyPort: CFStringDeprecated

let kCFStreamPropertyHTTPRequestBytesWrittenCount: CFStringDeprecated

let kCFStreamPropertyHTTPResponseHeader: CFString

HTTP Response Header property. When copied by CFReadStreamCopyProperty(_:_:), the header of an HTTP response message is returned.

Deprecated

let kCFStreamPropertyHTTPSProxyHost: CFStringDeprecated

let kCFStreamPropertyHTTPSProxyPort: CFStringDeprecated

let kCFStreamPropertyHTTPShouldAutoredirect: CFString

HTTP Should Auto Redirect property. Set this property to `kCFBooleanTrue` to enable autoredirection; set this property to `kCFBooleanFalse` to disable autoredirection.

Deprecated

func CFWriteStreamCreateWithFTPURL(CFAllocator?, CFURL) -> Unmanaged&lt;CFWriteStream>

Creates an FTP write stream.

Deprecated

func CFReadStreamCreateWithFTPURL(CFAllocator?, CFURL) -> Unmanaged&lt;CFReadStream>

Creates an FTP read stream.

Deprecated

