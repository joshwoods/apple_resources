

- SpriteKit
- SKVideoNode
-  init(videoURL:) Deprecated

Initializer

# init(videoURL:)

Initializes a video node using a URL that points to a video file.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedtvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**watchOS**

``` source
init(videoURL url: URL)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(videoURL url: URL)
```

Deprecated

Use init(url:) instead.

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

init(url: URL)

Initializes a video node using a URL.

init?(coder: NSCoder)

Tells you when to initialize a video node that was created from an archive.

init(videoFileNamed: String)

Initializes a video node using a video file stored in the app bundle.

Deprecated

