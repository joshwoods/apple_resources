

- SpriteKit
- SKVideoNode
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Initializes a video node using a video file stored in the app bundle.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 1.0+

**watchOS**

``` source
init(fileNamed videoFile: String)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(fileNamed videoFile: String)
```

## Parameters 

`videoFile`  

The name of the video file.

## Return Value

An initialized video node.

## See Also

### Creating a Video Node

init(avPlayer: AVPlayer)

Initializes a video node using an existing AVPlayer object.

init(url: URL)

Initializes a video node using a URL.

init?(coder: NSCoder)

Tells you when to initialize a video node that was created from an archive.

init(videoFileNamed: String)

Initializes a video node using a video file stored in the app bundle.

Deprecated

init(videoURL: URL)

Initializes a video node using a URL that points to a video file.

Deprecated

