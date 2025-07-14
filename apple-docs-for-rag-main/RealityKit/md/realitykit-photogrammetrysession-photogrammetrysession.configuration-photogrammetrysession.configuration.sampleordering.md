

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Configuration
-  PhotogrammetrySession.Configuration.SampleOrdering 

Enumeration

# PhotogrammetrySession.Configuration.SampleOrdering

The ordering of samples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
enum SampleOrdering
```

## Topics

### Specifying sample ordering

case unordered

Images aren’t in sequential order.

case sequential

Images are in sequential order.

### Comparing values

var hashValue: Int

The hash value.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (PhotogrammetrySession.Configuration.SampleOrdering, PhotogrammetrySession.Configuration.SampleOrdering) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Configuring sample ordering

var sampleOrdering: PhotogrammetrySession.Configuration.SampleOrdering

The order of the image samples.

