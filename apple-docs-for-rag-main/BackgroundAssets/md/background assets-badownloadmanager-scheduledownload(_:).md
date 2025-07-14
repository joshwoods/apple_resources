

- Background Assets
- BADownloadManager
-  scheduleDownload(\_:) 

Instance Method

# scheduleDownload(\_:)

Schedules an asset download to execute in the background at a nonspecific time in the future.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func scheduleDownload(_ download: BADownload) throws
```

## Parameters 

`download`  

The object that provides the URL of the asset to download.

## See Also

### Managing downloads

func startForegroundDownload(BADownload) throws

Schedules an asset download that executes immediately in the foreground.

func cancel(BADownload) throws

Cancels an asset download.

