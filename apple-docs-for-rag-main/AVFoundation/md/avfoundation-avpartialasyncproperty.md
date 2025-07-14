

- AVFoundation
-  AVPartialAsyncProperty 

Class

# AVPartialAsyncProperty

An asynchronous property that constrains its type.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
class AVPartialAsyncProperty
```

## Overview

This class defines the AVAsyncProperty constants for various AVFoundation types, including AVAsset, AVAssetTrack, and AVMetadataItem.

## Topics

### Loading Properties

AVAsset

Asynchronous properties for assets.

AVAssetTrack

Asynchronous properties for asset tracks.

AVURLAsset

Asynchronous properties for URL assets.

AVFragmentedAsset

Asynchronous properties for fragmented assets.

AVMetadataItem

Asynchronous properties for metadata items.

AVComposition

Asynchronous properties for compositions.

AVMutableComposition

Asynchronous properties for mutable compositions.

AVMovie

Asynchronous properties for movies.

AVMutableMovie

Asynchronous properties for mutable movies.

AVFragmentedMovie

Asynchronous properties for fragmented movies.

### Describing a Property

var description: String

A description of the object.

## Relationships

### Inherits From

- AVAnyAsyncProperty

### Inherited By

- AVAsyncProperty

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Property loading

protocol AVAsynchronousKeyValueLoading

A protocol that defines the interface to load media data asynchronously.

class AVAsyncProperty

An asynchronous property that constrains its type and value.

class AVAnyAsyncProperty

A base class for asynchronous properties.

