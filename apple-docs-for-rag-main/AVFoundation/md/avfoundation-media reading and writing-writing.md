

- AVFoundation
-  Media reading and writing 

API Collection

# Media reading and writing

Read images from video, export to alternative formats, and perform sample-level reading and writing of media data.

## Topics

### Media export

Exporting video to alternative formats

Convert an existing movie file to a different format.

class AVAssetExportSession

An object that exports assets in a format that you specify using an export preset.

### Image generation

Creating images from a video asset

Display images for specific times within the media timeline by generating images from a video’s frames.

class AVAssetImageGenerator

An object that generates images from a video asset.

### Media reading

Reading multiview 3D video files

Render single images for the left eye and right eye from a multiview High Efficiency Video Coding format file by reading individual video frames.

class AVAssetReader

An object that reads media data from an asset.

class AVAssetReaderOutput

An abstract class that defines the interface to read media samples from an asset reader.

class AVAssetReaderTrackOutput

An object that reads media data from a single track of an asset.

class AVAssetReaderAudioMixOutput

An object that reads audio samples that result from mixing audio from one or more tracks.

class AVAssetReaderVideoCompositionOutput

An object that reads composited video frames from one or more tracks of an asset.

class AVAssetReaderSampleReferenceOutput

An object that reads sample references from an asset track.

class AVAssetReaderOutputMetadataAdaptor

An object that creates timed metadata group objects for an asset track.

### Media writing

Writing Fragmented MPEG-4 Files for HTTP Live Streaming

Create an HTTP Live Streaming presentation by turning a movie file into a sequence of fragmented MPEG-4 files.

Converting side-by-side 3D video to multiview HEVC and spatial video

Create video content for visionOS by converting an existing 3D HEVC file to a multiview HEVC format, optionally adding spatial metadata to create a spatial video.

Creating spatial photos and videos with spatial metadata

Add spatial metadata to stereo photos and videos to create spatial media for viewing on Apple Vision Pro.

Tagging Media with Video Color Information

Inspect and set video color space information when writing and transcoding media.

Evaluating an App’s Video Color

Check color reproduction for a video in your app by using test patterns, video test equipment, and light-measurement instruments.

class AVOutputSettingsAssistant

An object that builds audio and video output settings dictionaries.

class AVAssetWriter

An object that writes media data to a container file.

class AVAssetWriterInput

An object that appends media samples to a track in an asset writer’s output file.

class AVAssetWriterInputPixelBufferAdaptor

An object that appends video samples to an asset writer input.

class AVAssetWriterInputTaggedPixelBufferGroupAdaptor

An object that appends tagged buffer groups to an asset writer input.

class AVAssetWriterInputMetadataAdaptor

An object that appends timed metadata groups to an asset writer input.

class AVAssetWriterInputGroup

A group of inputs with tracks that are mutually exclusive to each other for playback or processing.

### Captions

Caption Authoring

Create captions and subtitles in industry-standard formats.

## See Also

### Common

Media assets

Load media assets from files and streams to inspect their attributes, tracks, and embedded metadata.

Media types and utilities

Identify the types of content and file formats that AVFoundation supports.

Video settings

Configure video processing settings using standard key and value constants.

Audio settings

Configure audio processing settings using standard key and value constants.

