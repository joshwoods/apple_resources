

- Quartz
-  IKScannerDeviceViewTransferMode 

Enumeration

# IKScannerDeviceViewTransferMode

These constants determine how the scanner data is returned to the delegate. They are used by the transferMode property.

macOS 10.4+

``` source
@frozen
enum IKScannerDeviceViewTransferMode
```

## Topics

### Constants

case fileBased

The scanned content will be saved to the specified download directory.

case memoryBased

The scanned data is returned to the delegate as a `NSData` object.

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

enum IKScannerDeviceViewDisplayMode

These constants specify the display mode the scanner view will use. They are used by the mode property.

