

- ImageCaptureCore
- ICCameraDevice
-  requestUploadFile(\_:options:uploadDelegate:didUploadSelector:contextInfo:) Deprecated

Instance Method

# requestUploadFile(\_:options:uploadDelegate:didUploadSelector:contextInfo:)

Uploads a file to the camera.

macOS 10.4–14.0Deprecated

``` source
func requestUploadFile(
    _ fileURL: URL,
    options: [ICUploadOption : Any] = [:],
    uploadDelegate: Any,
    didUploadSelector selector: Selector,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Discussion

The `uploadDelegate` must implement a function with the signature `- (void)didUploadFile:(NSURL*)fileURL error:(NSError*)error contextInfo:(void*)contextInfo`, to be called when the request is completed.

## See Also

### Uploading Files

struct ICUploadOption

An option for uploading a file to the camera.

