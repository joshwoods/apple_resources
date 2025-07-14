

- SpriteKit
- SKVideoNode
-  init(url:) 

Initializer

# init(url:)

Initializes a video node using a URL.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
init(url: URL)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(url: URL)
```

## Parameters 

`url`  

The URL for the video to play.

## Return Value

An initialized video node.

## See Also

### Creating a Video Node

init(avPlayer: AVPlayer)

Initializes a video node using an existing AVPlayer object.

init(fileNamed: String)

Initializes a video node using a video file stored in the app bundle.

init?(coder: NSCoder)

Tells you when to initialize a video node that was created from an archive.

init(videoFileNamed: String)

Initializes a video node using a video file stored in the app bundle.

Deprecated

init(videoURL: URL)

Initializes a video node using a URL that points to a video file.

Deprecated

