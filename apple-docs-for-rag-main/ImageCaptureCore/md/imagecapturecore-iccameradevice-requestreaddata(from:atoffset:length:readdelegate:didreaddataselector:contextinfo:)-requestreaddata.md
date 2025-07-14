

- ImageCaptureCore
- ICCameraDevice
-  requestReadData(from:atOffset:length:readDelegate:didReadDataSelector:contextInfo:) 

Instance Method

# requestReadData(from:atOffset:length:readDelegate:didReadDataSelector:contextInfo:)

Asynchronously reads data of a specified length from a specified offset.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 10.4+visionOS 1.0+

``` source
func requestReadData(
    from file: ICCameraFile,
    atOffset offset: off_t,
    length: off_t,
    readDelegate: Any,
    didReadDataSelector selector: Selector,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Discussion

The `readDelegate` must implement a function with the signature `didReadData(data:NSData, fromFile:ICCameraFile, error:NSError, contextInfo:Any)`, to be called when the request is completed.

## See Also

### Reading Files

var contents: [ICCameraItem]?

All image, movie, and audio files stored on the camera, in an order that reflects the camera’s storage folder structure.

var mediaFiles: [ICCameraItem]?

All image, movie and audio files stored on the camera, without regard to the camera’s storage folder structure.

var contentCatalogPercentCompleted: Int

The percentage of the camera’s content that has been catalogued.

func files(ofType: String) -> [String]?

Returns an array of files of the selected type on the camera.

