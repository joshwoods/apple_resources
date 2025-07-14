

- RealityKit
- VideoPlayerComponent
-  VideoPlayerComponent.ImmersiveViewingMode 

Enumeration

# VideoPlayerComponent.ImmersiveViewingMode

Options for viewing the video during immersive-media playback.

visionOS 2.0+

``` source
enum ImmersiveViewingMode
```

## Overview

This applies only to immersive media types.

## Topics

### Operators

static func == (VideoPlayerComponent.ImmersiveViewingMode, VideoPlayerComponent.ImmersiveViewingMode) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case full

A viewing mode that renders immersive video covering the viewer’s entire field of view.

case portal

A viewing mode that renders immersive video as a portal window matching the containing entity’s transform.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Video player configurations

struct VideoPlayerComponent

A component that supports general video-playback experience with an AV player.

struct VideoMaterial

A material that supports animated textures.

class VideoPlaybackController

An object that controls the playback of video for a video material.

enum ViewingMode

Options for viewing video playback.

