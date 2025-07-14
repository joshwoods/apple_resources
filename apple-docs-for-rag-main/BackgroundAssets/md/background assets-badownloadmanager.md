

- Background Assets
-  BADownloadManager 

Class

# BADownloadManager

An object that manages the queue of scheduled asset downloads.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
class BADownloadManager
```

## Overview

Use BADownloadManager to schedule and cancel asset downloads, monitor their progress, and access the queue of pending downloads. You don’t create instances of this class directly; instead, use the shared property to access the framework’s singleton that it shares between your app and the app’s extension. Because the download manager is a shared resource, prevent race conditions by using the withExclusiveControl(_:) and withExclusiveControl(beforeDate:perform:) methods to assume absolute control of the manager before you schedule asset downloads or manipulate those already in the manager’s queue. To respond to asset download events and process concluded downloads, create a type that conforms to the BADownloadManagerDelegate protocol and assign an instance of it to the download manager’s delegate property.

The following example shows how to create an asset download, acquire exclusive control of the shared download manager, and then use the manager to schedule the download:

```
```

## Topics

### Accessing the download manager

class var shared: BADownloadManager

The download manager that both the app and the extension share.

### Managing downloads

func scheduleDownload(BADownload) throws

Schedules an asset download to execute in the background at a nonspecific time in the future.

func startForegroundDownload(BADownload) throws

Schedules an asset download that executes immediately in the foreground.

func cancel(BADownload) throws

Cancels an asset download.

### Monitoring downloads

var delegate: (any BADownloadManagerDelegate)?

The download manager’s delegate.

protocol BADownloadManagerDelegate

An interface for reacting to asset download events and processing concluded downloads.

### Fetching in-progress downloads

func fetchCurrentDownloads() throws -> [BADownload]

func fetchCurrentDownloads(completionHandler: ([BADownload], (any Error)?) -> Void)

Fetches the contents of the manager’s download queue.

### Synchronizing manager access

func withExclusiveControl((Bool, (any Error)?) -> Void)

Attempts to acquire immediate, exclusive access to the download manager.

func withExclusiveControl(beforeDate: Date, perform: (Bool, (any Error)?) -> Void)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Asset download management

protocol BADownloaderExtension

An interface for reacting to app life-cycle events and processing concluded asset downloads while your app isn’t running.

protocol BADownloaderExtensionConfiguration

Downloading essential assets in the background

Fetch the assets your app requires before its first launch using an app extension and the Background Assets framework.

