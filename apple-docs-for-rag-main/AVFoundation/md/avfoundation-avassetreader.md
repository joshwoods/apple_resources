

- AVFoundation
-  AVAssetReader 

Class

# AVAssetReader

An object that reads media data from an asset.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetReader
```

## Overview

Use an asset reader to read media data from instances of AVAsset. The assets you read may represent file-based media like QuickTime movies or MPEG-4 files, or media that you compose from multiple sources using AVComposition.

## Topics

### Creating an Asset Reader

init(asset: AVAsset) throws

Creates an object to read media data from an asset.

### Managing Outputs

func canAdd(AVAssetReaderOutput) -> Bool

Determines whether you can add the output to the asset reader.

func add(AVAssetReaderOutput)

Adds an output to the reader.

var outputs: [AVAssetReaderOutput]

The outputs from which you read media data.

### Configuring Reading

var timeRange: CMTimeRange

The time range within the asset to read.

var status: AVAssetReader.Status

The status of reading sample buffers from the asset.

enum Status

Values that represent the possible states of an asset reader.

var error: (any Error)?

An error that describes the reason for a failure.

### Controlling Reading

func startReading() -> Bool

Prepares the asset reader to start reading sample buffers from the asset.

func cancelReading()

Cancels any background work and stops the reader’s outputs from reading more samples.

### Inspecting the Asset

var asset: AVAsset

The asset from which to read media data.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media reading

Reading multiview 3D video files

Render single images for the left eye and right eye from a multiview High Efficiency Video Coding format file by reading individual video frames.

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

