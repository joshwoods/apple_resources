

- Background Assets
- BADownloadManagerDelegate
-  download(\_:failedWithError:) 

Instance Method

# download(\_:failedWithError:)

Informs the delegate about a failed asset download.

iOS 16.1+iPadOS 16.1+Mac Catalyst 16.1+macOS 13.0+tvOS 18.4+visionOS 2.4+

``` source
optional func download(
    _ download: BADownload,
    failedWithError error: any Error
)
```

## Parameters 

`download`  

The failed asset download.

`error`  

An object that provides detailed information about why the framework isn’t able to download the asset.

## See Also

### Processing concluded downloads

func download(BADownload, finishedWithFileURL: URL)

Informs the delegate about a finished asset download and provides the on-disk location.

