

- ARKit
- ARConfiguration
-  providesAudioData 

Instance Property

# providesAudioData

A Boolean value that specifies whether to capture audio during the AR session.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+

``` source
var providesAudioData: Bool { get set }
```

## Discussion

To receive and handle captured audio data, your session delegate must implement the session(_:didOutputAudioSampleBuffer:) method.

