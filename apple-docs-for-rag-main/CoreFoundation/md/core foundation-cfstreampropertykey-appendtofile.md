

- Core Foundation
- CFStreamPropertyKey
-  appendToFile 

Type Property

# appendToFile

Value is a `CFBoolean` value that indicates whether to append the written data to a file, if it already exists, rather than to replace its contents.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static let appendToFile: CFStreamPropertyKey!
```

## Discussion

You must set this value before opening the writable file stream. The default value is `kCFBooleanFalse`, indicating that the stream should replace any pre-existing file. You cannot read this value.

## See Also

### Constants

static let dataWritten: CFStreamPropertyKey!

Value is a `CFData` object that contains all the bytes written to a writable memory stream. You cannot modify this value.

static let fileCurrentOffset: CFStreamPropertyKey!

Value is a `CFNumber` object containing the current file offset.

static let socketNativeHandle: CFStreamPropertyKey!

Value is a `CFData` object that contains the native handle for a socket stream—of type CFSocketNativeHandle—to which the socket stream is connected.

static let socketRemoteHostName: CFStreamPropertyKey!

Value is a `CFString` object containing the name of the host to which the socket stream is connected or `NULL` if unknown.

static let socketRemotePortNumber: CFStreamPropertyKey!

Value is a `CFNumber` object containing the remote port number to which the socket stream is connected or `NULL` if unknown.

let kCFStreamPropertyShouldCloseNativeSocket: CFString

Should Close Native Socket property key.

let kCFStreamPropertySocketSecurityLevel: CFString

Socket Security Level property key.

let kCFStreamPropertySSLPeerCertificates: CFString

SSL Peer Certificates property key for copy operations, which return a \`CFArray\` object containing \`SecCertificateRef\` objects.

Deprecated

let kCFStreamPropertySSLPeerTrust: CFString

SSL Peer Trust property key for copy operations, which return a \`SecTrustRef\` object containing the result of the SSL handshake.

let kCFStreamPropertySSLSettings: CFString

SSL Settings property key for set operations.

let kCFStreamPropertySSLContext: CFString

let kCFStreamPropertySOCKSProxy: CFString

SOCKS proxy property key.

let kCFStreamPropertyProxyLocalBypass: CFString

Proxy Local Bypass property key.

let kCFStreamPropertySocketRemoteHost: CFString

The key’s value is a \`CFHostRef\` for the remote host if it is known. If not, its value is \`NULL\`.

let kCFStreamPropertySocketRemoteNetService: CFString

The key’s value is a \`CFNetServiceRef\` for the remote network service if it is known. If not, its value is \`NULL\`.

