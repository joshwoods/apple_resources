

- Core Media
-  CMPackingType 

Enumeration

# CMPackingType

The type of packing within each video frame, if any.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum CMPackingType
```

## Overview

Frame-packed video contains both the left and right eye images on a single video track. With frame-packed video, use the appropriate Frame Arrangement.

## Topics

### Frame Arrangement

case none

Each frame contains only a single image, and isn’t frame-packed.

case sideBySide

The video contains packed frames that have a left eye image on the left and right eye image on the right.

case overUnder

The video contains packed frames that have a left eye image on the top and right eye image on the bottom.

### Initializers

init?(rawValue: UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Metadata

CMMetadata APIs

The APIs for working with the framework’s Metadata Identifier Services and Metadata Data Type Registry.

CMTag APIs

Types and interfaces for working with Core Media tags.

class CMTag

A tag to set additional metadata on media buffers.

class CMTypedTag

A tag to set additional metadata on media buffers, with an associated Swift type for its value.

CMTagCollection APIs

Objective-C types and interfaces for working with Core Media tag collections.

enum CMProjectionType

Constants describing the projection surface information in a 3D video buffer or channel.

struct CMStereoViewComponents

Constants describing the stereo views contained within a buffer or channel.

struct CMStereoViewInterpretationOptions

Create a set of stereo view interpretation options from a constant.

