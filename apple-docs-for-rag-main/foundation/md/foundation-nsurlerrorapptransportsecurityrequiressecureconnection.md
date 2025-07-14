

- Foundation
-  NSURLErrorAppTransportSecurityRequiresSecureConnection 

Global Variable

# NSURLErrorAppTransportSecurityRequiresSecureConnection

App Transport Security disallowed a connection because there is no secure network connection.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var NSURLErrorAppTransportSecurityRequiresSecureConnection: Int { get }
```

## Discussion

Starting in iOS 9.0 and macOS v10.11, App Transport Security (ATS) is enabled by default for connections created by URLSession. ATS requires the use of best practice secure protocols in HTTPS. For more information on ATS, see NSAppTransportSecurity in Information Property List Key Reference.

## See Also

### URL Errors

var NSURLErrorBackgroundSessionInUseByAnotherProcess: Int

An app or app extension attempted to connect to a background session that is already connected to a process.

var NSURLErrorBackgroundSessionRequiresSharedContainer: Int

The shared container identifier of the URL session configuration is needed but hasn’t been set.

var NSURLErrorBackgroundSessionWasDisconnected: Int

The app is suspended or exits while a background data task is processing.

var NSURLErrorBadServerResponse: Int

The URL Loading System received bad data from the server.

var NSURLErrorBadURL: Int

A malformed URL prevented a URL request from being initiated.

var NSURLErrorCallIsActive: Int

A connection was attempted while a phone call was active on a network that doesn’t support simultaneous phone and data communication, such as EDGE or GPRS.

var NSURLErrorCancelled: Int

An asynchronous load has been canceled.

var NSURLErrorCannotCloseFile: Int

A download task couldn’t close the downloaded file on disk.

var NSURLErrorCannotConnectToHost: Int

An attempt to connect to a host failed.

var NSURLErrorCannotCreateFile: Int

A download task couldn’t create the downloaded file on disk because of an I/O failure.

var NSURLErrorCannotDecodeContentData: Int

Content data received during a connection request had an unknown content encoding.

var NSURLErrorCannotDecodeRawData: Int

Content data received during a connection request couldn’t be decoded for a known content encoding.

var NSURLErrorCannotFindHost: Int

The host name for a URL couldn’t be resolved.

var NSURLErrorCannotLoadFromNetwork: Int

A specific request to load an item only from the cache couldn’t be satisfied.

var NSURLErrorCannotMoveFile: Int

A downloaded file on disk couldn’t be moved.

