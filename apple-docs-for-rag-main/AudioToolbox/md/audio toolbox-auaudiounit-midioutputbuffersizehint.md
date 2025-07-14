

- Audio Toolbox
- AUAudioUnit
-  midiOutputBufferSizeHint 

Instance Property

# midiOutputBufferSizeHint

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var midiOutputBufferSizeHint: Int { get set }
```

## See Also

### Customizing the Audio Unit Behavior

class func registerSubclass(AnyClass, as: AudioComponentDescription, name: String, version: UInt32)

Registers an audio unit subclass.

func shouldChange(to: AVAudioFormat, for: AUAudioUnitBus) -> Bool

This is called when you set the format on a bus.

func setRenderResourcesAllocated(Bool)

Sets the Boolean value of the renderResourcesAllocated property.

var internalRenderBlock: AUInternalRenderBlock

The block which you must provide, via a getter, in order to implement rendering.

typealias AUInternalRenderBlock

A block to render the audio unit.

