

- SpriteKit
- SKVideoNode
-  init(avPlayer:) 

Initializer

# init(avPlayer:)

Initializes a video node using an existing AVPlayer object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
init(avPlayer player: AVPlayer)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(avPlayer player: AVPlayer)
```

## Parameters 

`player`  

A player object.

## Return Value

An initialized video node.

## Discussion

You can use the AVPlayer object to control playback.

Listing 1 shows, in Swift, how you can create a video node using the init(avPlayer:) initializer.

Listing 1. Creating a video node with an AV Player

```
var videoNode: SKVideoNode? = {
    guard let urlString = Bundle.main.path(forResource: "sample", ofType: "mov") else {
        return nil
    }

    let url = URL(fileURLWithPath: urlString)
    let item = AVPlayerItem(url: url)
    let player = AVPlayer(playerItem: item)

    return SKVideoNode(avPlayer: player)
}()
```

## See Also

### Creating a Video Node

init(fileNamed: String)

Initializes a video node using a video file stored in the app bundle.

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

