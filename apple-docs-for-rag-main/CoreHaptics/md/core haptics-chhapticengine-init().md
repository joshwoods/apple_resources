

- Core Haptics
- CHHapticEngine
-  init() 

Initializer

# init()

Creates an instance of the haptic engine.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init() throws
```

## Discussion

The haptic engine isn’t a singleton but a connection to the haptic server inside the user’s device. More than one connection with the haptic server may exist in your app’s view controller or delegate. Each connection functions independently of the others.

## See Also

### Initializing a Haptic Engine

init(audioSession: AVAudioSession?) throws

Creates a haptic engine from an audio session.

