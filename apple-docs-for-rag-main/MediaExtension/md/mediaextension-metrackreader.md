

- MediaExtension
-  METrackReader 

Protocol

# METrackReader

A protocol that defines the information to provide about a track within a media asset.

macOS 14.0+

``` source
protocol METrackReader : NSObjectProtocol
```

## Overview

Return default values for methods that don’t apply to a track type.

## Topics

### Getting track information

func loadTrackInfo(completionHandler: (METrackInfo?, (any Error)?) -> Void)

Loads the track info object with the properties of the media asset track.

**Required**

func generateSampleCursor(atPresentationTimeStamp: CMTime, completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the sample at or near the specified presentation timestamp.

**Required**

func generateSampleCursorAtFirstSampleInDecodeOrder(completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the first sample in decode order.

**Required**

func generateSampleCursorAtLastSampleInDecodeOrder(completionHandler: ((any MESampleCursor)?, (any Error)?) -> Void)

Provides a new sample cursor that points to the last sample in decode order.

**Required**

func loadUneditedDuration(completionHandler: (CMTime, (any Error)?) -> Void)

Returns the duration of the track, disregarding edits.

func loadTotalSampleDataLength(completionHandler: (Int64, (any Error)?) -> Void)

Loads the total size in bytes of all the samples in the track.

func loadEstimatedDataRate(completionHandler: (Float32, (any Error)?) -> Void)

Loads the approximate data rate of the track in bytes per second.

func loadMetadata(completionHandler: ([AVMetadataItem]?, (any Error)?) -> Void)

Loads the array of metadata items from the media asset track.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Track readers

class METrackInfo

An object that includes track properties parsed from the media asset.

