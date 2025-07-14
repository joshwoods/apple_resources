

- Create ML Components
- ImageFlipper
-  ImageFlipper.Orientation 

Enumeration

# ImageFlipper.Orientation

The orientation to flip the image.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
enum Orientation
```

## Topics

### Image orientations

case horizontal

Flip the image horizontally.

case vertical

Flip the image vertically.

### Operators

static func == (ImageFlipper.Orientation, ImageFlipper.Orientation) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating a transformer

init(orientation: ImageFlipper.Orientation)

Creates an image flipper.

