

- SpriteKit
- SKVideoNode
-  init(videoFileNamed:) Deprecated

Initializer

# init(videoFileNamed:)

Initializes a video node using a video file stored in the app bundle.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedtvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(videoFileNamed videoFile: String)
```

**watchOS**

``` source
init(videoFileNamed videoFile: String)
```

Deprecated

Use init(fileNamed:) instead.

## Parameters 

`videoFile`  

The name of the video file.

## Return Value

An initialized video node.

## See Also

### Creating a Video Node

init(avPlayer: AVPlayer)

Initializes a video node using an existing AVPlayer object.

init(fileNamed: String)

Initializes a video node using a video file stored in the app bundle.

init(url: URL)

Initializes a video node using a URL.

init?(coder: NSCoder)

Tells you when to initialize a video node that was created from an archive.

init(videoURL: URL)

Initializes a video node using a URL that points to a video file.

Deprecated

