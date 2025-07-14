

- Core Media
-  CMTag 

Class

# CMTag

A tag to set additional metadata on media buffers.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
class CMTag
```

## Overview

The Core Media framework uses tags to describe the properties of media channels. Each tag consists of a category and a value, both of which are 64 bits in size.

Important

Tag data can only contain values that can be safely stored on disk. In particular, CMTag values can’t contain a pointer. If you need to refer to another media element or in-memory data as part of a tag, use a buffer index or other constant.

It’s recommended to use CMTypedTag instances where possible to preserve type safety.

## Topics

### Creating Tags

static func channelID(Int64) -> CMTypedTag&lt;Int64>

Creates a new channel ID tag from an integer.

static func mediaSubType(CMFormatDescription.MediaSubType) -> CMTypedTag&lt;CMFormatDescription.MediaSubType>

Creates a tag containing media subtype metadata.

static func mediaType(CMFormatDescription.MediaType) -> CMTypedTag&lt;CMFormatDescription.MediaType>

Creates a tag containing media type metadata.

static func packingType(CMPackingType) -> CMTypedTag&lt;CMPackingType>

Creates a tag containing frame-packing information.

static func pixelFormat(OSType) -> CMTypedTag&lt;OSType>

Creates a tag containing pixel format information.

static func projectionType(CMProjectionType) -> CMTypedTag&lt;CMProjectionType>

Creates a tag containing projection surface information.

static func stereoView(CMStereoViewComponents) -> CMTypedTag&lt;CMStereoViewComponents>

Creates a tag containing eye information for 3D video.

static func stereoViewInterpretation(CMStereoViewInterpretationOptions) -> CMTypedTag&lt;CMStereoViewInterpretationOptions>

Creates a tag containing information on how to interpret stereo view metadata.

static func trackID(CMPersistentTrackID) -> CMTypedTag&lt;CMPersistentTrackID>

Creates a tag containing a track ID.

static func videoLayerID(Int64) -> CMTypedTag&lt;Int64>

Creates a tag containing a video layer ID.

init(rawCategory: CMTag.RawCategory, rawTagValue: CMTag.Value)

Creates a new tag from a category and value.

### Inspecting Tags

let rawCategory: CMTag.RawCategory

The raw 64-bit representation of the tag’s category.

let rawTagValue: CMTag.Value

The tag’s contained value.

func value&lt;T>(onlyIfMatching: CMTypedTag&lt;T>.Category) -> T?

Retrieves a tag’s value as a specific type, if and only if it matches a category.

### Wrapped Values

enum Value

A wrapper type for a value associated with a tag.

### Type Aliases

typealias RawCategory

The raw 64-bit representation of a tag’s category.

## Relationships

### Inherited By

- CMTypedTag

### Conforms To

- CustomStringConvertible
- Equatable
- Sendable

## See Also

### Metadata

CMMetadata APIs

The APIs for working with the framework’s Metadata Identifier Services and Metadata Data Type Registry.

CMTag APIs

Types and interfaces for working with Core Media tags.

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

enum CMPackingType

The type of packing within each video frame, if any.

