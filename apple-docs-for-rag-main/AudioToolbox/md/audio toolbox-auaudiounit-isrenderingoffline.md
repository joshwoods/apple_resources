

- Audio Toolbox
- AUAudioUnit
-  isRenderingOffline 

Instance Property

# isRenderingOffline

Communicates to an audio unit that it is rendering offline.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var isRenderingOffline: Bool { get set }
```

## Discussion

A host should use this property when using an audio unit in a context where there are no realtime deadlines. An audio unit may respond by using a more expensive signal processing algorithm, or allowing itself to block at render time if data being generated on secondary work threads is not ready in time.

This version 3 property is bridged to the version 2 `kAudioUnitProperty_OfflineRender` API.

## See Also

### Optimizing Performance

var latency: TimeInterval

The audio unit’s processing latency, in seconds.

var tailTime: TimeInterval

The audio unit’s tail time, in seconds.

var renderQuality: Int

Provides a trade-off between rendering quality and CPU load.

var shouldBypassEffect: Bool

Determines whether an effect should route input directly to output, without any processing.

var canProcessInPlace: Bool

Determines whether an audio unit can process in place.

