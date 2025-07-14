

- AVFoundation
-  AVCaptionRegion 

Class

# AVCaptionRegion

An object that represents the region in which the system presents a caption.

iOS 18.0+iPadOS 18.0+Mac Catalyst 15.0+macOS 12.0+

``` source
class AVCaptionRegion
```

## Overview

The framework defines four regions, and doesn’t support configuring region settings.

## Topics

### Accessing Defined Regions

class var appleITTTop: AVCaptionRegion

The top region for iTT format captions.

class var appleITTBottom: AVCaptionRegion

The bottom region for iTT format captions.

class var appleITTLeft: AVCaptionRegion

The left region for iTT format captions.

class var appleITTRight: AVCaptionRegion

The right region for iTT format captions.

class var subRipTextBottom: AVCaptionRegion

The bottom caption region for SubRip Text (SRT) format captions.

### Identifying a Region

var identifier: String?

A string that identifies the region.

### Accessing Dimensions

struct AVCaptionDimension

A structure that defines a caption dimension.

### Accessing the Location

var origin: AVCaptionPoint

The region’s top-left position.

struct AVCaptionPoint

A structure that defines the origin point for a caption.

### Accessing the Size

var size: AVCaptionSize

The height and width of the region.

struct AVCaptionSize

A structure that defines the height and width of a caption.

### Accessing the Display Alignment

var displayAlignment: AVCaptionRegion.DisplayAlignment

The alignment of lines for the region.

enum DisplayAlignment

Constants that indicate the alignment of lines in a region.

### Accessing the Scroll Mode

var scroll: AVCaptionRegion.Scroll

The scroll mode of the region.

enum Scroll

Constants that indicate the scrolling effects the system applies to a region.

### Accessing the Writing Mode

var writingMode: AVCaptionRegion.WritingMode

The block and inline progression direction of the region.

enum WritingMode

Constants that indicate the writing mode for a region.

### Processing Regions

func mutableCopy(with: NSZone?) -> Any

Creates a mutable copy of a caption region.

func encode(with: NSCoder)

Encodes the region using the specified encoder.

func isEqual(Any) -> Bool

Returns a Boolean value that indicates whether an object equals another.

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVMutableCaptionRegion

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Regions

class AVMutableCaptionRegion

A mutable caption region subclass that you use to create new caption regions.

