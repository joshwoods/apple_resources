

- AVFoundation
-  AVAssetCache 

Class

# AVAssetCache

An object that you use to inspect locally cached media data.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 10.0+

``` source
class AVAssetCache
```

## Overview

You can download HTTP Live Streaming assets to an iOS device using the AVAssetDownloadURLSession and AVAssetDownloadTask classes.

## Topics

### Inspecting the Cached Media

var isPlayableOffline: Bool

A Boolean value that indicates whether the asset is playable without an internet connection.

func mediaSelectionOptions(in: AVMediaSelectionGroup) -> [AVMediaSelectionOption]

Returns an array of locally cached media selection options that are available for offline use.

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
- Sendable

