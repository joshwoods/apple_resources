

- SpriteKit
- SKAudioNode
-  init(avAudioNode:) 

Initializer

# init(avAudioNode:)

Initializes an audio node from an AVFoundation audio node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init(avAudioNode node: AVAudioNode?)
```

**watchOS**

``` source
init(avAudioNode node: AVAudioNode?)
```

## Parameters 

`node`  

An AVAudioNode object that holds an AVAudioEngine sound graph from a single sound source or URL.

## Return Value

A newly initialized audio node.

## See Also

### Initializing Audio Nodes

convenience init(fileNamed: String)

Initializes an audio node from an audio asset with the specified filename.

convenience init(url: URL)

Initializes an audio node from an audio asset with the specified URL.

init?(coder: NSCoder)

Tells you when to initialize an audio node that has been unarchived.

