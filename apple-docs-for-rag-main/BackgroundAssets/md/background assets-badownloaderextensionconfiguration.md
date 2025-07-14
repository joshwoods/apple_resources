

- Background Assets
-  BADownloaderExtensionConfiguration 

Protocol

# BADownloaderExtensionConfiguration

iOS 16.1+iPadOS 16.1+Mac CatalystmacOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
@MainActor @preconcurrency
protocol BADownloaderExtensionConfiguration : AppExtensionConfiguration
```

## Relationships

### Inherits From

- AppExtensionConfiguration
- Sendable

## See Also

### Asset download management

class BADownloadManager

An object that manages the queue of scheduled asset downloads.

protocol BADownloaderExtension

An interface for reacting to app life-cycle events and processing concluded asset downloads while your app isn’t running.

Downloading essential assets in the background

Fetch the assets your app requires before its first launch using an app extension and the Background Assets framework.

