

- SpriteKit
- SKVideoNode
-  init(coder:) 

Initializer

# init(coder:)

Tells you when to initialize a video node that was created from an archive.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
init?(coder aDecoder: NSCoder)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init?(coder aDecoder: NSCoder)
```

## Discussion

Do not call this initializer yourself; it is called by the system when you should intialize a video node that was created from an archive.

## See Also

### Creating a Video Node

init(avPlayer: AVPlayer)

Initializes a video node using an existing AVPlayer object.

init(fileNamed: String)

Initializes a video node using a video file stored in the app bundle.

init(url: URL)

Initializes a video node using a URL.

init(videoFileNamed: String)

Initializes a video node using a video file stored in the app bundle.

Deprecated

init(videoURL: URL)

Initializes a video node using a URL that points to a video file.

Deprecated

