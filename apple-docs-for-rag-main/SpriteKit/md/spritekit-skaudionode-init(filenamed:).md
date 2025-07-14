

- SpriteKit
- SKAudioNode
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Initializes an audio node from an audio asset with the specified filename.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

**watchOS**

``` source
convenience init(fileNamed name: String)
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
convenience init(fileNamed name: String)
```

## Parameters 

`name`  

A file containing an AVAudioNode.

## Return Value

A newly initialized audio node.

## Discussion

The named file containing the audio asset must reside within the main bundle.

## See Also

### Initializing Audio Nodes

init(avAudioNode: AVAudioNode?)

Initializes an audio node from an AVFoundation audio node.

convenience init(url: URL)

Initializes an audio node from an audio asset with the specified URL.

init?(coder: NSCoder)

Tells you when to initialize an audio node that has been unarchived.

