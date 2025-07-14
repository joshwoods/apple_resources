

- SpriteKit
- SKSpriteNode
-  init(coder:) 

Initializer

# init(coder:)

Tells you when to initialize a sprite from an archive.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
init?(coder aDecoder: NSCoder)
```

**watchOS**

``` source
init?(coder aDecoder: NSCoder)
```

## Discussion

Don’t call this function directly; the system calls this function when you should initialize your sprite from the argument archived data.

