

- SpriteKit
- SKAudioNode
-  init(coder:) 

Initializer

# init(coder:)

Tells you when to initialize an audio node that has been unarchived.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

Do not call this initializer directly; it’s called by the system when you should initialize an audio node that has been unarchived.

## See Also

### Initializing Audio Nodes

init(avAudioNode: AVAudioNode?)

Initializes an audio node from an AVFoundation audio node.

convenience init(fileNamed: String)

Initializes an audio node from an audio asset with the specified filename.

convenience init(url: URL)

Initializes an audio node from an audio asset with the specified URL.

