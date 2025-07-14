

- RealityKit
- VideoMaterial
-  init(avPlayer:) 

Initializer

# init(avPlayer:)

Creates a new video material.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
@MainActor @preconcurrency
init(avPlayer: AVPlayer)
```

## Parameters 

`avPlayer`  

An AVPlayer instance.

## Discussion

To create a video material, first create an AVPlayer instance initialized with a URL that points to the movie file you want the video material to play, then pass that to this initializer. The following code demonstrates this process.

```
// Create a URL that points to the movie file.
if let url = Bundle.main.url(forResource: "MyMovie", withExtension: "mp4") {

    // Create an AVPlayer instance to control playback of that movie.
    let player = AVPlayer(url: url)

    // Instantiate and configure the video material.
    let material = VideoMaterial(avPlayer: player)

    // Configure audio playback mode. This is optional for movie
    // files that contain sound.
    material.controller.audioInputMode = .spatial

    // Create a new model entity using the video material.
    let modelEntity = ModelEntity(mesh: cube, materials: [material])

    // Start playing the video.
    player.play()
}
```

