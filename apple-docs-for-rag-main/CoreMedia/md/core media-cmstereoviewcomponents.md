

- Core Media
-  CMStereoViewComponents 

Structure

# CMStereoViewComponents

Constants describing the stereo views contained within a buffer or channel.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct CMStereoViewComponents
```

## Overview

When no stereo view components are available on a video track, even if it’s encoded for multiview video, any video content in the associated data is single-track 2D.

## Topics

### Eye Layer

static var leftEye: CMStereoViewComponents

The stereo video track includes a left eye layer.

static var rightEye: CMStereoViewComponents

The stereo video track includes a right eye layer.

### Initializers

init(rawValue: UInt64)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

struct CMStereoViewInterpretationOptions

Create a set of stereo view interpretation options from a constant.

enum CMPackingType

The type of packing within each video frame, if any.

