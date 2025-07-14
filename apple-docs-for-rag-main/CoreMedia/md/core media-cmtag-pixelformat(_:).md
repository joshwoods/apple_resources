

- Core Media
- CMTag
-  pixelFormat(\_:) 

Type Method

# pixelFormat(\_:)

Creates a tag containing pixel format information.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func pixelFormat(_ value: OSType) -> CMTypedTag
```

## Parameters 

`value`  

The pixel format for this tag. Use a constant from the framework that renders video content. For example, rendering to a CVPixelBuffer should use a constant from Pixel Format Identifiers.

## Return Value

A new typed tag containing the pixel format represented by `value`.

## See Also

### Creating Tags

static func channelID(Int64) -> CMTypedTag&lt;Int64>

Creates a new channel ID tag from an integer.

static func mediaSubType(CMFormatDescription.MediaSubType) -> CMTypedTag&lt;CMFormatDescription.MediaSubType>

Creates a tag containing media subtype metadata.

static func mediaType(CMFormatDescription.MediaType) -> CMTypedTag&lt;CMFormatDescription.MediaType>

Creates a tag containing media type metadata.

static func packingType(CMPackingType) -> CMTypedTag&lt;CMPackingType>

Creates a tag containing frame-packing information.

static func projectionType(CMProjectionType) -> CMTypedTag&lt;CMProjectionType>

Creates a tag containing projection surface information.

static func stereoView(CMStereoViewComponents) -> CMTypedTag&lt;CMStereoViewComponents>

Creates a tag containing eye information for 3D video.

static func stereoViewInterpretation(CMStereoViewInterpretationOptions) -> CMTypedTag&lt;CMStereoViewInterpretationOptions>

Creates a tag containing information on how to interpret stereo view metadata.

static func trackID(CMPersistentTrackID) -> CMTypedTag&lt;CMPersistentTrackID>

Creates a tag containing a track ID.

static func videoLayerID(Int64) -> CMTypedTag&lt;Int64>

Creates a tag containing a video layer ID.

init(rawCategory: CMTag.RawCategory, rawTagValue: CMTag.Value)

Creates a new tag from a category and value.

