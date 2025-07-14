

- Vision
-  VNVideoProcessingOption Deprecated

Structure

# VNVideoProcessingOption

Options to pass to the video processor when adding requests.

iOS 14.0–14.0DeprecatediPadOS 14.0–14.0DeprecatedMac Catalyst 14.0–14.0DeprecatedmacOS 11.0–11.0DeprecatedtvOS 14.0–14.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
struct VNVideoProcessingOption
```

## Topics

### Options

static let frameCadence: VNVideoProcessingOption

A value that indicates the video frame cadence at which to perform the video processing.

static let timeInterval: VNVideoProcessingOption

A value that indicates that the video processor should perform a request every *n*-seconds.

### Initializers

init(rawValue: String)

Creates an option with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

