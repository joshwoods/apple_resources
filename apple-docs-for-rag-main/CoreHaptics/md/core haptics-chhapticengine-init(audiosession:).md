

- Core Haptics
- CHHapticEngine
-  init(audioSession:) 

Initializer

# init(audioSession:)

Creates a haptic engine from an audio session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(audioSession: AVAudioSession?) throws
```

## Parameters 

`audioSession`  

The shared audio session, if you’re already using one in your app, to sync with the created engine. For example, pass in sharedInstance() if you’re using audio from AVAudioSession. Pass in `nil` to use default UIKit audio behavior.

## Discussion

Create your haptic engine with this initializer if you want the audio behavior of your engine to match other audio APIs in your app. For example, if you’re using AVAudioSession to manage audio elsewhere in your app, then you want to share the session’s sharedInstance(). In this case, the engine mutes and routes audio in accordance with the passed session.

Otherwise, if you don’t pass it a session, it won’t behave the same way as elsewhere in app; audio behaves like UIKit, without syncing to a specific session. You should pass `nil` when you need the engine only for playing haptics.

## See Also

### Initializing a Haptic Engine

init() throws

Creates an instance of the haptic engine.

