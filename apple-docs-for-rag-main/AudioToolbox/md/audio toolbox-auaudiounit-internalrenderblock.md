

- Audio Toolbox
- AUAudioUnit
-  internalRenderBlock 

Instance Property

# internalRenderBlock

The block which you must provide, via a getter, in order to implement rendering.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var internalRenderBlock: AUInternalRenderBlock { get }
```

## See Also

### Customizing the Audio Unit Behavior

class func registerSubclass(AnyClass, as: AudioComponentDescription, name: String, version: UInt32)

Registers an audio unit subclass.

func shouldChange(to: AVAudioFormat, for: AUAudioUnitBus) -> Bool

This is called when you set the format on a bus.

func setRenderResourcesAllocated(Bool)

Sets the Boolean value of the renderResourcesAllocated property.

var midiOutputBufferSizeHint: Int

typealias AUInternalRenderBlock

A block to render the audio unit.

