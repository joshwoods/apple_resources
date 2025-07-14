

- Foundation
- URLError
-  cannotCloseFile 

Type Property

# cannotCloseFile

A download task couldn’t close the downloaded file on disk.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var cannotCloseFile: URLError.Code { get }
```

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

static var cannotMoveFile: URLError.Code

A download task was unable to move a downloaded file on disk.

