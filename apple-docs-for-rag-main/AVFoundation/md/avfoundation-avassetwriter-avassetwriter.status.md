

- AVFoundation
- AVAssetWriter
-  AVAssetWriter.Status 

Enumeration

# AVAssetWriter.Status

Values that indicate the state of an asset writer.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum Status
```

## Topics

### Status Values

case unknown

The asset writer’s status isn’t known.

case writing

The asset writer is writing.

case completed

The asset writer finishes writing successfully.

case failed

The asset writer fails to write the output file.

case cancelled

The asset writer canceled the writing operation.

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

### Inspecting Writing Status

var status: AVAssetWriter.Status

The status of writing samples to the output file.

var error: (any Error)?

An error object that describes an asset-writing failure.

