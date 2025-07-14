

- ARKit
- ARSessionObserver
-  session(\_:didOutputAudioSampleBuffer:) 

Instance Method

# session(\_:didOutputAudioSampleBuffer:)

Tells the delegate that a new sample buffer of recorded audio is available.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
optional func session(
    _ session: ARSession,
    didOutputAudioSampleBuffer audioSampleBuffer: CMSampleBuffer
)
```

## Parameters 

`session`  

The session providing information.

`audioSampleBuffer`  

The sample buffer that was output.

## Discussion

ARKit calls this method on your delegate object only if you’re running an AR session with a configuration whose providesAudioData setting is true.

