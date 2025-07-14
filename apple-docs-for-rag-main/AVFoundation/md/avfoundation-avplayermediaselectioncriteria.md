

- AVFoundation
-  AVPlayerMediaSelectionCriteria 

Class

# AVPlayerMediaSelectionCriteria

An object that specifies the preferred languages and media characteristics for a player.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class AVPlayerMediaSelectionCriteria
```

## Overview

An instance of this object represents the languages and media characteristics of assets that contain media selection options that a player attempts to select automatically when preparing and playing items. It lists the languages and media characteristics in their preferred order.

## Topics

### Creating Media Selection Criteria

init(preferredLanguages: [String]?, preferredMediaCharacteristics: [AVMediaCharacteristic]?)

Creates media selection criteria with the preferred languages and media characteristics.

init(principalMediaCharacteristics: [AVMediaCharacteristic]?, preferredLanguages: [String]?, preferredMediaCharacteristics: [AVMediaCharacteristic]?)

Creates media selection criteria with the principal media characteristics, and preferred languages and media characteristics.

### Retrieving Selection Criteria Settings

var preferredLanguages: [String]?

An array of language identifiers in preferred order.

var preferredMediaCharacteristics: [AVMediaCharacteristic]?

An array of media characteristics in preferred order.

var principalMediaCharacteristics: [AVMediaCharacteristic]?

An array of media characteristics that are essential to select when choosing media with a particular characteristic.

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

## See Also

### Media selection

Selecting Subtitles and Alternative Audio Tracks

Extend your app’s appeal to users by adding subtitles and alternative audio tracks in their native language.

class AVMediaSelection

An object that represents a complete rendition of media selection options on an asset.

class AVMediaSelectionGroup

An object that represents a collection of mutually exclusive options for the presentation of media within an asset.

class AVMediaSelectionOption

An object that represents a specific option for the presentation of media within a group of options.

class AVMutableMediaSelection

A mutable object that represents a complete rendition of media selection options on an asset.

