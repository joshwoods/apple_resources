

- Audio Toolbox
- AUAudioUnit
-  shouldBypassEffect 

Instance Property

# shouldBypassEffect

Determines whether an effect should route input directly to output, without any processing.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var shouldBypassEffect: Bool { get set }
```

## Discussion

This version 3 property is bridged to the version 2 `kAudioUnitProperty_BypassEffect` API.

## See Also

### Optimizing Performance

var latency: TimeInterval

The audio unit’s processing latency, in seconds.

var tailTime: TimeInterval

The audio unit’s tail time, in seconds.

var renderQuality: Int

Provides a trade-off between rendering quality and CPU load.

var canProcessInPlace: Bool

Determines whether an audio unit can process in place.

var isRenderingOffline: Bool

Communicates to an audio unit that it is rendering offline.

