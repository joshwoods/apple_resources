

- CFNetwork
-  CFWriteStreamCreateWithFTPURL(\_:\_:) Deprecated

Function

# CFWriteStreamCreateWithFTPURL(\_:\_:)

Creates an FTP write stream.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.3–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func CFWriteStreamCreateWithFTPURL(
    _ alloc: CFAllocator?,
    _ ftpURL: CFURL
) -> Unmanaged
```

Deprecated

Use NSURLSessionAPI for ftp requests

## Parameters 

`alloc`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`ftpURL`  

A pointer to a CFURL structure for the URL to be uploaded created by calling any of the `CFURLCreate` functions, such as `CFURLCreateWithString`.

## Return Value

A new write stream, or `NULL` if the call failed. Ownership follows the The Create Rule.

## Discussion

This function creates an FTP write stream for uploading data to an FTP URL. If the `ftpURL` parameter is created with the user name and password as part of the URL (such as `ftp://username:password@ftp.example.com`) then the user name and password will automatically be set in the `CFWriteStream`. Call CFWriteStreamSetProperty(_:_:_:) to set the steam’s properties, such as `kCFStreamPropertyFTPUserName` and `kCFStreamPropertyFTPPassword` to associate a user name and password with the stream that are used to log in when the stream is opened. See `Constants` for a description of all FTP stream properties.

After creating the write stream, you can call CFWriteStreamGetStatus(_:) at any time to check the status of the stream.

To initiate a connection with the FTP server, call CFWriteStreamOpen(_:). If the URL specifies a directory, the open is immediately followed by the event `kCFStreamEventEndEncountered` (and the stream passes to the state `kCFStreamStatusAtEnd`). Once the stream reaches this state, the directory has been created. Intermediary directories are not created.

To write to the FTP stream, call CFWriteStreamWrite(_:_:_:).

To close a connection with the FTP server, call CFWriteStreamClose(_:).

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

func CFReadStreamCreateWithFTPURL(CFAllocator?, CFURL) -> Unmanaged&lt;CFReadStream>

Creates an FTP read stream.

Deprecated

let kCFStreamPropertyFTPAttemptPersistentConnection: CFStringDeprecated

