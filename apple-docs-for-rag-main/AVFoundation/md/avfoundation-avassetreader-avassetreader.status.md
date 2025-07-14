

- AVFoundation
- AVAssetReader
-  AVAssetReader.Status 

Enumeration

# AVAssetReader.Status

Values that represent the possible states of an asset reader.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
enum Status
```

## Overview

You determine an asset reader’s status using its status property.

## Topics

### Status Values

case unknown

The asset reader is in an unknown state.

case reading

The asset reader is successfully reading samples from its asset.

case completed

The asset reader completes reading all samples within its specified time range.

case failed

The asset reader can no longer read samples from its asset because of an error.

case cancelled

The asset reader can no longer read samples because you canceled reading.

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

### Configuring Reading

var timeRange: CMTimeRange

The time range within the asset to read.

var status: AVAssetReader.Status

The status of reading sample buffers from the asset.

var error: (any Error)?

An error that describes the reason for a failure.

