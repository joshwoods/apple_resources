

- Vision
-  VNChirality 

Enumeration

# VNChirality

Constants that the define the chirality, or handedness, of a pose.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
@frozen
enum VNChirality
```

## Topics

### Chirality Values

case left

Indicates a left-handed pose.

case right

Indicates a right-handed pose.

case unknown

Indicates that the pose chirality is unknown.

### Creating a Chirality

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Determining the Chirality

var chirality: VNChirality

The chirality, or handedness, of a pose.

