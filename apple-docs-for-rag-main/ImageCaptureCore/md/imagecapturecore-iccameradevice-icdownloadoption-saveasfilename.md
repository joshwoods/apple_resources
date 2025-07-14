

- ImageCaptureCore
- ICCameraDevice
- ICDownloadOption
-  saveAsFilename 

Type Property

# saveAsFilename

The name to be used for the downloaded file.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
static let saveAsFilename: ICDownloadOption
```

## Discussion

Specify the filename as an NSString object.

## See Also

### Download Options

static let downloadsDirectoryURL: ICDownloadOption

A writable directory where the downloaded files should be saved.

static let savedFilename: ICDownloadOption

The actual name of the saved file.

static let savedAncillaryFiles: ICDownloadOption

An array of files associated with the file being downloaded.

static let overwrite: ICDownloadOption

A Boolean value indicating whether the downloaded file should overwrite an existing file with the same name and extension.

static let deleteAfterSuccessfulDownload: ICDownloadOption

A Boolean value indicating whether to delete the file from the device after a successful download.

static let sidecarFiles: ICDownloadOption

A Boolean value indicating whether to download all sidecar files along with the media file.

