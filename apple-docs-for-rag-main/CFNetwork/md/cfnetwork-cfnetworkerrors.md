

- CFNetwork
-  CFNetworkErrors 

Enumeration

# CFNetworkErrors

This enumeration contains error codes returned under the error domain kCFErrorDomainCFNetwork.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.8+tvOS 9.0+visionOS 1.0+

``` source
enum CFNetworkErrors
```

## Overview

To determine the source of an error, examine the `userInfo` dictionary included in the `CFError` object returned by a function call or call CFErrorGetDomain(_:) and pass in the `CFError` object and the domain whose value you want to read. These errors are all part of the `kCFErrorDomainCFNetwork` domain.

## Topics

### Constants

case cfHostErrorHostNotFound

The specified host wasn’t found.

case cfHostErrorUnknown

An unknown error.

case cfsocksErrorUnknownClientVersion

The SOCKS server rejected access because it doesn’t support connections with the requested SOCKS version.

case cfsocksErrorUnsupportedServerVersion

The SOCKS server doesn’t support the requested version.

case cfsocks4ErrorRequestFailed

The server rejected the request, or the request failed.

case cfsocks4ErrorIdentdFailed

The server couldn’t connect to the `identd` daemon on the client and rejected the request.

case cfsocks4ErrorIdConflict

The server rejected the request because the client program and the `identd` daemon reported different user IDs.

case cfsocks4ErrorUnknownStatusCode

The server returned an unknown status code.

case cfsocks5ErrorBadState

The stream isn’t in a state that allows the requested operation.

case cfsocks5ErrorBadResponseAddr

The address type returned isn’t supported.

case cfsocks5ErrorBadCredentials

The SOCKS server refused the client connection because of bad login credentials.

case cfsocks5ErrorUnsupportedNegotiationMethod

The requested method isn’t supported.

case cfsocks5ErrorNoAcceptableMethod

The client and server couldn’t find a mutually agreeable authentication method.

case cfftpErrorUnexpectedStatusCode

The server returned an unexpected status code.

case cfErrorHTTPAuthenticationTypeUnsupported

The client and server couldn’t agree on a supported authentication type.

case cfErrorHTTPBadCredentials

The server rejected the credentials provided for an authenticated connection.

case cfErrorHTTPConnectionLost

The connection to the server was dropped.

case cfErrorHTTPParseFailure

The HTTP server response couldn’t be parsed.

case cfErrorHTTPRedirectionLoopDetected

Too many HTTP redirects occurred before reaching a page that didn’t redirect the client to another page.

case cfErrorHTTPBadURL

The requested URL couldn’t be retrieved.

case cfErrorHTTPProxyConnectionFailure

A connection to the HTTPS proxy couldn’t be established.

case cfErrorHTTPBadProxyCredentials

The proxy rejected the authentication credentials provided for logging in.

case cfErrorPACFileError

An error occurred with the proxy autoconfiguration file.

case cfErrorPACFileAuth

The authentication credentials provided by the proxy autoconfiguration file were rejected.

case cfErrorHTTPSProxyConnectionFailure

A connection couldn’t be established to the HTTPS proxy.

case cfStreamErrorHTTPSProxyFailureUnexpectedResponseToCONNECTMethod

The HTTPS proxy returned an unexpected status code, such as a `3xx` redirect.

case cfurlErrorUnknown

An unknown error occurred.

case cfurlErrorCancelled

The connection was cancelled.

case cfurlErrorBadURL

The connection failed due to a malformed URL.

case cfurlErrorTimedOut

The connection timed out.

case cfurlErrorUnsupportedURL

The connection failed due to an unsupported URL scheme.

case cfurlErrorCannotFindHost

The connection failed because the host couldn’t be found.

case cfurlErrorCannotConnectToHost

The connection failed because a connection can’t be made to the host.

case cfurlErrorNetworkConnectionLost

The connection failed because the network connection was lost.

case cfurlErrorDNSLookupFailed

The connection failed because the DNS lookup failed.

case cfurlErrorHTTPTooManyRedirects

The HTTP connection failed due to too many redirects.

case cfurlErrorResourceUnavailable

The connection’s resource is unavailable.

case cfurlErrorNotConnectedToInternet

The connection failed because the device isn’t connected to the internet.

case cfurlErrorRedirectToNonExistentLocation

The connection was redirected to a nonexistent location.

case cfurlErrorBadServerResponse

The connection received an invalid server response.

case cfurlErrorUserCancelledAuthentication

The connection failed because the user cancelled required authentication.

case cfurlErrorUserAuthenticationRequired

The connection failed because it requires authentication.

case cfurlErrorZeroByteResource

The resource retrieved by the connection is zero bytes.

case cfurlErrorCannotDecodeRawData

The connection can’t decode data encoded with a known content encoding.

case cfurlErrorCannotDecodeContentData

The connection can’t decode data encoded with an unknown content encoding.

case cfurlErrorCannotParseResponse

The connection can’t parse the server’s response.

case cfurlErrorInternationalRoamingOff

The connection failed because international roaming is disabled on the device.

case cfurlErrorCallIsActive

The connection failed because a call is active.

case cfurlErrorDataNotAllowed

The connection failed because data use isn’t currently allowed on the device.

case cfurlErrorRequestBodyStreamExhausted

The connection failed because the request’s body stream was exhausted.

case cfurlErrorFileDoesNotExist

The file operation failed because the file doesn’t exist.

case cfurlErrorFileIsDirectory

The file operation failed because the file is a directory.

case cfurlErrorNoPermissionsToReadFile

The file operation failed because it doesn’t have permission to read the file.

case cfurlErrorDataLengthExceedsMaximum

The file operation failed because the file is too large.

case cfurlErrorSecureConnectionFailed

The secure connection failed for an unknown reason.

case cfurlErrorServerCertificateHasBadDate

The secure connection failed because the server’s certificate has an invalid date.

case cfurlErrorServerCertificateUntrusted

The secure connection failed because the server’s certificate isn’t trusted.

case cfurlErrorServerCertificateHasUnknownRoot

The secure connection failed because the server’s certificate has an unknown root.

case cfurlErrorServerCertificateNotYetValid

The secure connection failed because the server’s certificate isn’t valid yet.

case cfurlErrorClientCertificateRejected

The secure connection failed because the client’s certificate was rejected.

case cfurlErrorClientCertificateRequired

The secure connection failed because the server requires a client certificate.

case cfurlErrorCannotLoadFromNetwork

The connection failed because it’s being required to return a cached resource, but one isn’t available.

case cfurlErrorCannotCreateFile

The file can’t be created.

case cfurlErrorCannotOpenFile

The file can’t be opened.

case cfurlErrorCannotCloseFile

The file can’t be closed.

case cfurlErrorCannotWriteToFile

The file can’t be written.

case cfurlErrorCannotRemoveFile

The file can’t be removed.

case cfurlErrorCannotMoveFile

The file can’t be moved.

case cfurlErrorDownloadDecodingFailedMidStream

The download failed because decoding of the downloaded data failed midstream.

case cfurlErrorDownloadDecodingFailedToComplete

The download failed because decoding of the downloaded data failed to complete.

case cfhttpCookieCannotParseCookieFile

The cookie file can’t be parsed.

case cfNetServiceErrorUnknown

An error of unknown type has occurred.

case cfNetServiceErrorCollision

An attempt was made to use a name that’s already in use.

case cfNetServiceErrorNotFound

This error isn’t used.

case cfNetServiceErrorInProgress

A new search couldn’t be started because a search is already in progress.

case cfNetServiceErrorBadArgument

A required argument either wasn’t provided or wasn’t valid.

case cfNetServiceErrorCancel

The search or service was canceled.

case cfNetServiceErrorInvalid

Invalid data was passed to a CFNetServices function.

case cfNetServiceErrorTimeout

Resolution failed because the timeout was reached.

case cfNetServiceErrorDNSServiceFailure

The DNS service discovery returned an error.

case cfurlErrorAppTransportSecurityRequiresSecureConnection

The connection failed because the App Transport Security configuration requires a secure connection.

case cfurlErrorBackgroundSessionInUseByAnotherProcess

The background session failed because it was in use by another process.

case cfurlErrorBackgroundSessionWasDisconnected

The background session failed because it was disconnected.

### Enumeration Cases

case cfurlErrorFileOutsideSafeArea

The file is outside of the safe area.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Errors

Error Dictionary Keys

Networking-related keys that may be available in a `CFErrorRef` object’s `userInfo` dictionary.

Error Domains

High-level error domains.

