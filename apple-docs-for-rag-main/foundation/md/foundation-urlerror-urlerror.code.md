

- Foundation
- URLError
-  URLError.Code 

Structure

# URLError.Code

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct Code
```

## Topics

### Error codes

static var appTransportSecurityRequiresSecureConnection: URLError.Code

App Transport Security disallowed a connection because there is no secure network connection.

static var backgroundSessionInUseByAnotherProcess: URLError.Code

An app or app extension attempted to connect to a background session that is already connected to a process.

static var backgroundSessionRequiresSharedContainer: URLError.Code

The shared container identifier of the URL session configuration is needed but has not been set.

static var backgroundSessionWasDisconnected: URLError.Code

The app is suspended or exits while a background data task is processing.

static var badServerResponse: URLError.Code

The URL Loading system received bad data from the server.

static var badURL: URLError.Code

A malformed URL prevented a URL request from being initiated.

static var callIsActive: URLError.Code

A connection was attempted while a phone call is active on a network that does not support simultaneous phone and data communication (EDGE or GPRS).

static var cancelled: URLError.Code

An asynchronous load has been canceled.

static var cannotCloseFile: URLError.Code

A download task couldn’t close the downloaded file on disk.

static var cannotConnectToHost: URLError.Code

An attempt to connect to a host failed.

static var cannotCreateFile: URLError.Code

A download task couldn’t create the downloaded file on disk because of an I/O failure.

static var cannotDecodeContentData: URLError.Code

Content data received during a connection request had an unknown content encoding.

static var cannotDecodeRawData: URLError.Code

Content data received during a connection request could not be decoded for a known content encoding.

static var cannotFindHost: URLError.Code

The host name for a URL could not be resolved.

static var cannotLoadFromNetwork: URLError.Code

A request to load an item only from the cache could not be satisfied.

static var cannotMoveFile: URLError.Code

A download task was unable to move a downloaded file on disk.

static var cannotOpenFile: URLError.Code

A download task was unable to open the downloaded file on disk.

static var cannotParseResponse: URLError.Code

A task could not parse a response.

static var cannotRemoveFile: URLError.Code

A download task was unable to remove a downloaded file from disk.

static var cannotWriteToFile: URLError.Code

A download task was unable to write to the downloaded file on disk.

static var clientCertificateRejected: URLError.Code

A server certificate was rejected.

static var clientCertificateRequired: URLError.Code

A client certificate was required to authenticate an SSL connection during a request.

static var dataLengthExceedsMaximum: URLError.Code

The length of the resource data exceeds the maximum allowed.

static var dataNotAllowed: URLError.Code

The cellular network disallowed a connection.

static var dnsLookupFailed: URLError.Code

The host address could not be found via DNS lookup.

static var downloadDecodingFailedMidStream: URLError.Code

A download task failed to decode an encoded file during the download.

static var downloadDecodingFailedToComplete: URLError.Code

A download task failed to decode an encoded file after downloading.

static var fileDoesNotExist: URLError.Code

A file does not exist.

static var fileIsDirectory: URLError.Code

A request for an FTP file resulted in the server responding that the file is not a plain file, but a directory.

static var httpTooManyRedirects: URLError.Code

A redirect loop has been detected or the threshold for number of allowable redirects has been exceeded (currently 16).

static var internationalRoamingOff: URLError.Code

The attempted connection required activating a data context while roaming, but international roaming is disabled.

static var networkConnectionLost: URLError.Code

A client or server connection was severed in the middle of an in-progress load.

static var noPermissionsToReadFile: URLError.Code

A resource couldn’t be read because of insufficient permissions.

static var notConnectedToInternet: URLError.Code

A network resource was requested, but an internet connection has not been established and cannot be established automatically.

static var redirectToNonExistentLocation: URLError.Code

A redirect was specified by way of server response code, but the server did not accompany this code with a redirect URL.

static var requestBodyStreamExhausted: URLError.Code

A body stream is needed but the client did not provide one.

static var resourceUnavailable: URLError.Code

A requested resource couldn’t be retrieved.

static var secureConnectionFailed: URLError.Code

An attempt to establish a secure connection failed for reasons that can’t be expressed more specifically.

static var serverCertificateHasBadDate: URLError.Code

A server certificate had a date which indicates it has expired, or is not yet valid.

static var serverCertificateHasUnknownRoot: URLError.Code

A server certificate was not signed by any root server.

static var serverCertificateNotYetValid: URLError.Code

A server certificate is not yet valid.

static var serverCertificateUntrusted: URLError.Code

A server certificate was signed by a root server that isn’t trusted.

static var timedOut: URLError.Code

An asynchronous operation timed out.

static var unknown: URLError.Code

The URL Loading System encountered an error that it can’t interpret.

static var unsupportedURL: URLError.Code

A properly formed URL couldn’t be handled by the framework.

static var userAuthenticationRequired: URLError.Code

Authentication is required to access a resource.

static var userCancelledAuthentication: URLError.Code

An asynchronous request for authentication has been canceled by the user.

static var zeroByteResource: URLError.Code

A server reported that a URL has a non-zero content length, but terminated the network connection gracefully without sending any data.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Error codes

static var appTransportSecurityRequiresSecureConnection: URLError.Code

App Transport Security disallowed a connection because there is no secure network connection.

static var backgroundSessionInUseByAnotherProcess: URLError.Code

An app or app extension attempted to connect to a background session that is already connected to a process.

static var backgroundSessionRequiresSharedContainer: URLError.Code

The shared container identifier of the URL session configuration is needed but hasn’t been set.

static var backgroundSessionWasDisconnected: URLError.Code

The app is suspended or exits while a background data task is processing.

static var badServerResponse: URLError.Code

The URL Loading System received bad data from the server.

static var badURL: URLError.Code

A malformed URL prevented a URL request from being initiated.

static var callIsActive: URLError.Code

A connection was attempted while a phone call is active on a network that doesn’t support simultaneous phone and data communication, such as EDGE or GPRS.

static var cancelled: URLError.Code

An asynchronous load has been canceled.

static var cannotCloseFile: URLError.Code

A download task couldn’t close the downloaded file on disk.

static var cannotConnectToHost: URLError.Code

An attempt to connect to a host failed.

static var cannotCreateFile: URLError.Code

A download task couldn’t create the downloaded file on disk because of an I/O failure.

static var cannotDecodeContentData: URLError.Code

Content data received during a connection request had an unknown content encoding.

static var cannotDecodeRawData: URLError.Code

Content data received during a connection request couldn’t be decoded for a known content encoding.

static var cannotFindHost: URLError.Code

The host name for a URL couldn’t be resolved.

static var cannotLoadFromNetwork: URLError.Code

A request to load an item only from the cache could not be satisfied.

