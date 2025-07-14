

- RealityKit
-  VideoMaterial 

Structure

# VideoMaterial

A material that supports animated textures.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
struct VideoMaterial
```

## Overview

In RealityKit, a *material* is an object that defines the surface properties of a rendered 3D object. A `VideoMaterial` is a material that maps a movie file on to the surface of an entity. Video materials are *unlit*, which means that scene lighting doesn’t affect them. Video materials support transparency if the source video’s file format also supports transparency.

Video materials use an AVPlayer instance to control movie playback. You can use any movie file format that AVPlayer supports to create a video material. To control playback of the material’s video, use the avPlayer property, which offers methods like play() and pause().

The following code demonstrates how to create and start playing a video material using a movie file from your application bundle.

```
// Create a URL that points to the movie file.
if let url = Bundle.main.url(forResource: "MyMovie", withExtension: "mp4") {

    // Create an AVPlayer instance to control playback of that movie.
    let player = AVPlayer(url: url)

    // Instantiate and configure the video material.
    let material = VideoMaterial(avPlayer: player)

    // Configure audio playback mode.
    material.controller.audioInputMode = .spatial

    // Create a new model entity using the video material.
    let modelEntity = ModelEntity(mesh: cube, materials: [material])

    // Start playing the video.
    player.play()
}
```

To see an example of using a video texture in RealityKit, see Creating a game with scene understanding.

## Topics

### Creating a video material

init(avPlayer: AVPlayer)

Creates a new video material.

### Controlling playback

var avPlayer: AVPlayer?

The material’s video playback controller.

var controller: VideoPlaybackController

An object that configures framework-specific video options.

### Initializers

init(videoRenderer: AVSampleBufferVideoRenderer)

Creates and initializes a video material for a sample buffer video renderer object.

### Instance Properties

var faceCulling: VideoMaterial.FaceCulling

A process in which the system specifies polygons to remove before rendering a mesh using this material.

var readsDepth: Bool

A boolean value that determines whether this material performs the depth test by reading RealityKit’s depth buffer.

var triangleFillMode: VideoMaterial.TriangleFillMode

The object that controls how RealityKit draws triangles.

var videoRenderer: AVSampleBufferVideoRenderer?

The material’s video renderer.

var writesDepth: Bool

A boolean value that determines whether this material writes its depth into RealityKit’s depth buffer.

### Type Aliases

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

### Default Implementations

Material Implementations

## Relationships

### Conforms To

- Material

## See Also

### Video materials

typealias FaceCulling

An alias for the cull mode object that’s appropriate for this material class.

typealias TriangleFillMode

typealias Parameters

The parameter type that custom materials uses for properties the framework passes to shader functions.

