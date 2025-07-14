

- Audio Toolbox
- AUAudioUnit
-  renderQuality 

Instance Property

# renderQuality

Provides a trade-off between rendering quality and CPU load.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var renderQuality: Int { get set }
```

## Discussion

The range of valid values is 0 to 127.

This version 3 property is bridged to the version 2 `kAudioUnitProperty_RenderQuality` API.

## See Also

### Optimizing Performance

var latency: TimeInterval

The audio unit’s processing latency, in seconds.

var tailTime: TimeInterval

The audio unit’s tail time, in seconds.

var shouldBypassEffect: Bool

Determines whether an effect should route input directly to output, without any processing.

var canProcessInPlace: Bool

Determines whether an audio unit can process in place.

var isRenderingOffline: Bool

Communicates to an audio unit that it is rendering offline.

