

- CFNetwork
-  CFStreamCreatePairWithSocketToCFHost(\_:\_:\_:\_:\_:) Deprecated

Function

# CFStreamCreatePairWithSocketToCFHost(\_:\_:\_:\_:\_:)

Creates readable and writable streams connected to a given `CFHost` object.

iOS 2.0–16.0DeprecatediPadOS 2.0–16.0DeprecatedMac Catalyst 13.1+macOS 10.3–15.0DeprecatedtvOS 9.0+visionOS 1.0–2.0Deprecated

``` source
func CFStreamCreatePairWithSocketToCFHost(
    _ alloc: CFAllocator?,
    _ host: CFHost,
    _ port: Int32,
    _ readStream: UnsafeMutablePointer?>?,
    _ writeStream: UnsafeMutablePointer?>?
)
```

Deprecated

Use Network framework instead

## Parameters 

`alloc`  

The allocator to use to allocate memory for the `CFReadStream` and `CFWriteStream` objects. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`host`  

A `CFHost` object to which the streams are connected. If unresolved, the host will be resolved prior to connecting.

`port`  

The TCP port number to which the socket streams should connect.

`readStream`  

Upon return, contains a `CFReadStream` object connected to the host `host` on port `port`, or `NULL` if there is a failure during creation. If you pass `NULL`, the function will not create a readable stream. Ownership follows the The Create Rule.

`writeStream`  

Upon return, contains a `CFWriteStream` object connected to the host `host` on port `port`, or `NULL` if there is a failure during creation. If you pass `NULL`, the function will not create a writable stream. Ownership follows the The Create Rule.

## Discussion

The streams do not create a socket or connect to the specified host until you open one of the streams.

Most properties are shared by both streams. Setting a shared property for one stream automatically sets the property for the other.

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

