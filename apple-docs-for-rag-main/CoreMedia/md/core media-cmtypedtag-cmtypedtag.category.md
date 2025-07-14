

- Core Media
- CMTypedTag
-  CMTypedTag.Category 

Structure

# CMTypedTag.Category

An identifier for a media tag category.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Category
```

## Topics

### Creating Typed Categories

static var channelID: CMTypedTag&lt;Int64>.Category

A category used for tagging a channel ID.

static var mediaSubType: CMTypedTag&lt;CMFormatDescription.MediaSubType>.Category

A category used for tagging media subtype metadata.

static var mediaType: CMTypedTag&lt;CMFormatDescription.MediaType>.Category

A category used for tagging media type metadata.

static var packingType: CMTypedTag&lt;CMPackingType>.Category

A category used for tagging frame-packing information.

static var pixelFormat: CMTypedTag&lt;OSType>.Category

A category used for tagging pixel format information.

static var projectionType: CMTypedTag&lt;CMProjectionType>.Category

A category used for tagging projection surface information.

static var stereoView: CMTypedTag&lt;CMStereoViewComponents>.Category

A category used for tagging eye information for 3D video.

static var stereoViewInterpretation: CMTypedTag&lt;CMStereoViewInterpretationOptions>.Category

A category used for tagging how to interpret stereo view metadata.

static var trackID: CMTypedTag&lt;CMPersistentTrackID>.Category

A category used for tagging a track ID.

static var videoLayerID: CMTypedTag&lt;Int64>.Category

A category used for tagging a video layer ID.

### Getting Raw Categories

let rawCategory: CMTypedTag&lt;TypedValue>.RawCategory

The raw 64-bit representation of the tag’s category.

### Transforming Tag Values

func tagValue(for: TypedValue) -> CMTag.Value

Convert a typed value to a raw tag value for this category.

func value(for: CMTag.Value) -> TypedValue?

Convert a tag value into a typed value valid for this category, if possible.

### Initializers

init(rawCategory: CMTypedTag&lt;TypedValue>.RawCategory, valueForTagValue: (CMTag.Value) -> TypedValue?, tagValueForValue: (TypedValue) -> CMTag.Value)

Creates a new tag category instance with defined mappings between a raw and typed tag value.

## Relationships

### Conforms To

- Sendable

