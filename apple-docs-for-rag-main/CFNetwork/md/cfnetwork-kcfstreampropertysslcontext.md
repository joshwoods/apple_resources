

- CFNetwork
-  kCFStreamPropertySSLContext 

Global Variable

# kCFStreamPropertySSLContext

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
let kCFStreamPropertySSLContext: CFString
```

## Discussion

The `SSLContextRef` object used for read and write operations on a stream.

Before opening a stream, you can copy the object from this property and configure it using the Secure Transport API. You can also set this property to specify a new `SSLContextRef` for a stream. The behavior depends on whether the stream has been opened and on whether an SSL context is associated with the stream, as follows:

- If the stream has not been opened, the specified object replaces any existing context, and is used in the initial stream handshake when the connection is opened.

- If the stream has been opened without SSL enabled, setting this property initiates an SSL handshake over the existing socket.

- After the initial SSL handshake occurs, changing the context object is unsupported.

If an SSL settings dictionary is set for the `kCFStreamPropertySSLSettings` key, an `SSLContextRef` object is created internally and configured based on that dictionary. However, if an `SSLContextRef` object is set afterwards, its configuration takes precedence over the previously configured context.

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

