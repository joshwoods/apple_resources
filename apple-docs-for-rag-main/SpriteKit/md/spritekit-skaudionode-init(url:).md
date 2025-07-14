

- SpriteKit
- SKAudioNode
-  init(url:) 

Initializer

# init(url:)

Initializes an audio node from an audio asset with the specified URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
convenience init(url: URL)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(url: URL)
```

## Parameters 

`url`  

The URL of an audio file.

## Return Value

A newly initialized audio node.

## See Also

### Initializing Audio Nodes

init(avAudioNode: AVAudioNode?)

Initializes an audio node from an AVFoundation audio node.

convenience init(fileNamed: String)

Initializes an audio node from an audio asset with the specified filename.

init?(coder: NSCoder)

Tells you when to initialize an audio node that has been unarchived.

