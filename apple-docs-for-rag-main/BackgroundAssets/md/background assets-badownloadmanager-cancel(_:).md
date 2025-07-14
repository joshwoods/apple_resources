

- Background Assets
- BADownloadManager
-  cancel(\_:) 

Instance Method

# cancel(\_:)

Cancels an asset download.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
func cancel(_ download: BADownload) throws
```

## Parameters 

`download`  

The object that identifies the scheduled or in-progress download to cancel.

## See Also

### Managing downloads

func scheduleDownload(BADownload) throws

Schedules an asset download to execute in the background at a nonspecific time in the future.

func startForegroundDownload(BADownload) throws

Schedules an asset download that executes immediately in the foreground.

