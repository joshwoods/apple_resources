

- Background Assets
-  BADownloaderExtension 

Protocol

# BADownloaderExtension

An interface for reacting to app life-cycle events and processing concluded asset downloads while your app isn’t running.

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
protocol BADownloaderExtension : AppExtension
```

## Topics

### Processing downloads

func backgroundDownload(BADownload, didReceive: URLAuthenticationChallenge) async -> (URLSession.AuthChallengeDisposition, URLCredential?)

**Required** Default implementation provided.

func backgroundDownload(BADownload, finishedWithFileURL: URL)

**Required** Default implementation provided.

func backgroundDownload(BADownload, failedWithError: any Error)

**Required** Default implementation provided.

### Checking for asset updates

func downloads(for: BAContentRequest, manifestURL: URL, extensionInfo: BAAppExtensionInfo) -> Set&lt;BADownload>

**Required** Default implementation provided.

enum BAContentRequest

class BAAppExtensionInfo

### Reacting to extension events

func extensionWillTerminate()

### Instance Methods

func extensionWillTerminate()

This method may be called shortly before the extension is terminated.

**Required** Default implementation provided.

## Relationships

### Inherits From

- AppExtension

## See Also

### Asset download management

class BADownloadManager

An object that manages the queue of scheduled asset downloads.

protocol BADownloaderExtensionConfiguration

Downloading essential assets in the background

Fetch the assets your app requires before its first launch using an app extension and the Background Assets framework.

