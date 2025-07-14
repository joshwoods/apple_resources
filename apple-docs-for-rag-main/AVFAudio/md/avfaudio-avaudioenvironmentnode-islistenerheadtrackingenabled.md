

- AVFAudio
- AVAudioEnvironmentNode
-  isListenerHeadTrackingEnabled 

Instance Property

# isListenerHeadTrackingEnabled

A Boolean value that indicates whether the listener orientation is automatically rotated based on head orientation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+

``` source
var isListenerHeadTrackingEnabled: Bool { get set }
```

## Discussion

To enable head tracking, your app must have the com.apple.developer.coremotion.head-pose entitlement.

Set this value to true to enable head tracking with compatible AirPods.

