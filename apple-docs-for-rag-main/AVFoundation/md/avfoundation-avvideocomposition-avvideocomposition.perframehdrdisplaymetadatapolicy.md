

- AVFoundation
- AVVideoComposition
-  AVVideoComposition.PerFrameHDRDisplayMetadataPolicy 

Structure

# AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

A type that defines the policy for handling of per frame HDR metadata.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct PerFrameHDRDisplayMetadataPolicy
```

## Discussion

Use this type to specify what HDR display metadata to attach to the rendered frame.

## Topics

### Policies

static let propagate: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

A policy that passes HDR metadata through, if present on the composed frame.

static let generate: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

A video composition may generate HDR metadata and attach it to the rendered frame.

### Initializers

init(rawValue: String)

Creates a policy with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring HDR Metadata

var perFrameHDRDisplayMetadataPolicy: AVVideoComposition.PerFrameHDRDisplayMetadataPolicy

Configures the policy for display of HDR display metadata on the rendered frame.

