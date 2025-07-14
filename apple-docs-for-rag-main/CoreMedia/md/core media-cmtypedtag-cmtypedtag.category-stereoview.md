

- Core Media
- CMTypedTag
- CMTypedTag.Category
-  stereoView 

Type Property

# stereoView

A category used for tagging eye information for 3D video.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var stereoView: CMTypedTag.Category { get }
```

Available when `TypedValue` conforms to `Sendable`.

## See Also

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

static var stereoViewInterpretation: CMTypedTag&lt;CMStereoViewInterpretationOptions>.Category

A category used for tagging how to interpret stereo view metadata.

static var trackID: CMTypedTag&lt;CMPersistentTrackID>.Category

A category used for tagging a track ID.

static var videoLayerID: CMTypedTag&lt;Int64>.Category

A category used for tagging a video layer ID.

