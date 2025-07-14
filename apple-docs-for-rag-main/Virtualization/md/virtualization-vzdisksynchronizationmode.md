

- Virtualization
-  VZDiskSynchronizationMode 

Enumeration

# VZDiskSynchronizationMode

Values that describe the synchronization modes available to the guest OS.

macOS 14.0+

``` source
enum VZDiskSynchronizationMode
```

## Topics

### Synchronization modes

case full

Perform all synchronization operations as requested by the guest OS.

case none

Don’t synchronize the data with the permanent storage.

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

### Virtual disk synchronization modes

enum VZDiskImageSynchronizationMode

An integer that describes the disk image synchronization mode.

