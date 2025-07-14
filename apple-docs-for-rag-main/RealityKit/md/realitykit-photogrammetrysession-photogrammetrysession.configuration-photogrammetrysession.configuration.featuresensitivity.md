

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  PhotogrammetrySession.Configuration.FeatureSensitivity 

Enumeration

# PhotogrammetrySession.Configuration.FeatureSensitivity

The sensitivity to sample landmarks.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum FeatureSensitivity
```

## Topics

### Specifying feature sensitivity

case normal

The session uses the default algorithm to detect landmarks.

case high

The session uses a slower, more sensitive algorithm to detect landmarks.

### Comparing values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (PhotogrammetrySession.Configuration.FeatureSensitivity, PhotogrammetrySession.Configuration.FeatureSensitivity) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring feature sensitivity

var featureSensitivity: PhotogrammetrySession.Configuration.FeatureSensitivity

The precision of landmark detection.

