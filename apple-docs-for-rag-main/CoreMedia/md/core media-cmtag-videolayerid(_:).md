

- Core Media
- CMTag
-  videoLayerID(\_:) 

Type Method

# videoLayerID(\_:)

Creates a tag containing a video layer ID.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func videoLayerID(_ value: Int64) -> CMTypedTag
```

## Parameters 

`value`  

The video layer ID for this tag.

## Return Value

A new typed tag containing a video layer ID of `value`.

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

static func pixelFormat(OSType) -> CMTypedTag&lt;OSType>

Creates a tag containing pixel format information.

static func projectionType(CMProjectionType) -> CMTypedTag&lt;CMProjectionType>

Creates a tag containing projection surface information.

static func stereoView(CMStereoViewComponents) -> CMTypedTag&lt;CMStereoViewComponents>

Creates a tag containing eye information for 3D video.

static func stereoViewInterpretation(CMStereoViewInterpretationOptions) -> CMTypedTag&lt;CMStereoViewInterpretationOptions>

Creates a tag containing information on how to interpret stereo view metadata.

static func trackID(CMPersistentTrackID) -> CMTypedTag&lt;CMPersistentTrackID>

Creates a tag containing a track ID.

init(rawCategory: CMTag.RawCategory, rawTagValue: CMTag.Value)

Creates a new tag from a category and value.

