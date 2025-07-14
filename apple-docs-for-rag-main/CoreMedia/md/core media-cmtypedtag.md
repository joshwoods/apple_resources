

- Core Media
-  CMTypedTag 

Class

# CMTypedTag

A tag to set additional metadata on media buffers, with an associated Swift type for its value.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class CMTypedTag where TypedValue : Sendable
```

## Topics

### Creating Typed Tags

init(category: CMTypedTag&lt;TypedValue>.Category, value: TypedValue)

Creates a new instance with the given category and value.

### Inspecting Typed Tags

let category: CMTypedTag&lt;TypedValue>.Category

The category of the tag.

var value: TypedValue

The value of the tag, represented as its appropriate type.

### Typed Tag Categories

struct Category

An identifier for a media tag category.

## Relationships

### Inherits From

- CMTag

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Metadata

CMMetadata APIs

The APIs for working with the framework’s Metadata Identifier Services and Metadata Data Type Registry.

CMTag APIs

Types and interfaces for working with Core Media tags.

class CMTag

A tag to set additional metadata on media buffers.

CMTagCollection APIs

Objective-C types and interfaces for working with Core Media tag collections.

enum CMProjectionType

Constants describing the projection surface information in a 3D video buffer or channel.

struct CMStereoViewComponents

Constants describing the stereo views contained within a buffer or channel.

struct CMStereoViewInterpretationOptions

Create a set of stereo view interpretation options from a constant.

enum CMPackingType

The type of packing within each video frame, if any.

