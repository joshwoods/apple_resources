

- Quartz
-  IKCameraDeviceViewTransferMode 

Enumeration

# IKCameraDeviceViewTransferMode

These constants specify the transfer mode used by the camera view. These constants are used by mode.

macOS 10.4+

``` source
@frozen
enum IKCameraDeviceViewTransferMode
```

## Topics

### Constants

case fileBased

Transferred files will be saved to disk by the delegate.

case memoryBased

Transferred files will be supplied to the delegate as an `NSData` object.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum IKCameraDeviceViewDisplayMode

These constants specify the display mode used by the camera view. These constants are used by mode.

