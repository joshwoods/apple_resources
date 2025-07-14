

- AVFoundation
-  AVAssetTrackGroupOutputHandling 

Structure

# AVAssetTrackGroupOutputHandling

A type that specifies policies for how an export session processes alternate tracks in a track group.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
struct AVAssetTrackGroupOutputHandling
```

## Topics

### Policies

static var preserveAlternateTracks: AVAssetTrackGroupOutputHandling

A policy that passes through alternate audio tracks from the source asset during export.

### Initializers

init(rawValue: UInt)

Creates track group output handling structure with a raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring Track Groups

var audioTrackGroupHandling: AVAssetTrackGroupOutputHandling

A policy that defines how the session exports alternate audio tracks.

