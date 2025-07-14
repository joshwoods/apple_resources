

- Audio Toolbox
- AUAudioUnit
-  registerSubclass(\_:as:name:version:) 

Type Method

# registerSubclass(\_:as:name:version:)

Registers an audio unit subclass.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
class func registerSubclass(
    _ cls: AnyClass,
    as componentDescription: AudioComponentDescription,
    name: String,
    version: UInt32
)
```

## Parameters 

`cls`  

An AUAudioUnit subclass.

`componentDescription`  

The component to register.

`name`  

The component’s name, using the convention `:`.

`version`  

The component’s version.

## Discussion

This method dynamically registers the supplied AUAudioUnit subclass with the Audio Component system, in the context of the current process only. After you’ve registered the subclass, instantiate it by calling one of the following:

- The init(componentDescription:) method.

- The init(componentDescription:options:) method.

- The AVAudioUnit instantiate(with:options:completionHandler:) method.

- The AudioComponentInstanceNew(_:_:) function.

## See Also

### Customizing the Audio Unit Behavior

func shouldChange(to: AVAudioFormat, for: AUAudioUnitBus) -> Bool

This is called when you set the format on a bus.

func setRenderResourcesAllocated(Bool)

Sets the Boolean value of the renderResourcesAllocated property.

var internalRenderBlock: AUInternalRenderBlock

The block which you must provide, via a getter, in order to implement rendering.

var midiOutputBufferSizeHint: Int

typealias AUInternalRenderBlock

A block to render the audio unit.

