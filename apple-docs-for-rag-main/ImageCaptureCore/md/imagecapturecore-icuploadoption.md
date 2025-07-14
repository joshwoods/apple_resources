

- ImageCaptureCore
-  ICUploadOption 

Structure

# ICUploadOption

An option for uploading a file to the camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
struct ICUploadOption
```

## Topics

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Uploading Files

func requestUploadFile(URL, options: [ICUploadOption : Any], uploadDelegate: Any, didUploadSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Uploads a file to the camera.

Deprecated

