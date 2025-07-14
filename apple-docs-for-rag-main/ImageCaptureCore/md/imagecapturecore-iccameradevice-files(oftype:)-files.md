

- ImageCaptureCore
- ICCameraDevice
-  files(ofType:) 

Instance Method

# files(ofType:)

Returns an array of files of the selected type on the camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func files(ofType fileUTType: String) -> [String]?
```

## Discussion

For the `fileType` parameter, pass one of the following uniform type identifier strings: `kUTTypeImage`, `kUTTypeMovie`, `kUTTypeAudio`, or `kUTTypeData`.

## See Also

### Reading Files

var contents: [ICCameraItem]?

All image, movie, and audio files stored on the camera, in an order that reflects the camera’s storage folder structure.

var mediaFiles: [ICCameraItem]?

All image, movie and audio files stored on the camera, without regard to the camera’s storage folder structure.

var contentCatalogPercentCompleted: Int

The percentage of the camera’s content that has been catalogued.

func requestReadData(from: ICCameraFile, atOffset: off_t, length: off_t, readDelegate: Any, didReadDataSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Asynchronously reads data of a specified length from a specified offset.

