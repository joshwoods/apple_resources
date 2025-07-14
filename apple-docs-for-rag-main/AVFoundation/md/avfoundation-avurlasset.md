

- AVFoundation
-  AVURLAsset 

Class

# AVURLAsset

An asset that represents media at a local or remote URL.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVURLAsset
```

## Overview

This class is a concrete subclass of AVAsset. When you create an asset as shown below, the system creates and returns an instance of AVURLAsset.

```
// A local or remote asset URL.
guard let url: URL = Bundle.main.url(forResource: "Image",
                                     withExtension: "png") else { return }
let asset = AVAsset(url: url)
```

In many cases, this is an appropriate way to create asset instances, but you can also directly instantiate an AVURLAsset when you need more fine-grained control over its initialization. The initializer for AVURLAsset accepts an options dictionary, which you use to customize the asset’s initialization for your particular purpose. For example, if you’re creating an asset for an HLS stream, you may want to prevent it from retrieving its media when it connects over a cellular network. You can do this by providing the initialization option and value as shown below.

```
let url: URL = // A remote asset URL.
let options = [AVURLAssetAllowsCellularAccessKey: false]
let asset = AVURLAsset(url: url, options: options)
```

## Topics

### Creating an Asset

convenience init(url: URL)

Creates an asset that models the media at the specified URL.

init(url: URL, options: [String : Any]?)

Creates an asset that models the media resource at the specified URL.

Initialization Options

Specify options to configure the initialization of a media asset.

### Loading Tracks

static var tracks: AVAsyncProperty&lt;Root, [AVAssetTrack]>

The tracks an asset contains.

func findCompatibleTrack(for: AVCompositionTrack, completionHandler: (AVAssetTrack?, (any Error)?) -> Void)

Loads an asset track from which you can insert any time range into the composition track.

### Loading Variants

static var variants: AVAsyncProperty&lt;Root, [AVAssetVariant]>

An array of variants that an asset contains.

### Determining Supported Media Types

class func audiovisualTypes() -> [AVFileType]

Returns an array of the file types the asset supports.

class func audiovisualMIMETypes() -> [String]

Returns an array of the MIME types the asset supports.

class func isPlayableExtendedMIMEType(String) -> Bool

Returns a Boolean value that indicates whether the asset is playable with the specified codecs and container type.

### Assisting with Resource Loading

var resourceLoader: AVAssetResourceLoader

The resource loader for the asset.

var mayRequireContentKeysForMediaDataProcessing: Bool

A Boolean value that indicates whether you can add this asset as a content key recipient to a content key session.

### Working with Offline Assets

var assetCache: AVAssetCache?

The asset’s associated asset cache, if it exists.

### Accessing the Media URL

var url: URL

A URL to the asset’s media.

### Accessing Asset Variants

var variants: [AVAssetVariant]

An array of variants that an asset contains.

Deprecated

### Accessing Compatible Tracks

func compatibleTrack(for: AVCompositionTrack) -> AVAssetTrack?

Returns an asset track from which you can insert any time range into a given composition track.

Deprecated

### Accessing the Session Identifier

var httpSessionIdentifier: UUID

A session identifier that the asset sends in HTTP requests that it makes.

### Accessing Media Extension Properties

var mediaExtensionProperties: AVMediaExtensionProperties?

The properties of the media extension format reader that decodes the asset.

class AVMediaExtensionProperties

An object that describes a Media Extension.

## Relationships

### Inherits From

- AVAsset

### Inherited By

- AVFragmentedAsset

### Conforms To

- AVAsynchronousKeyValueLoading
- AVContentKeyRecipient
- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSItemProviderReading
- NSItemProviderWriting
- NSObjectProtocol
- Sendable

## See Also

### Assets

class AVAsset

An object that models timed audiovisual media.

class AVAssetTrack

An object that models a track of media that an asset contains.

class AVAssetTrackSegment

An object that represents a time range segment of an asset track.

class AVAssetTrackGroup

A group of related tracks in an asset.

