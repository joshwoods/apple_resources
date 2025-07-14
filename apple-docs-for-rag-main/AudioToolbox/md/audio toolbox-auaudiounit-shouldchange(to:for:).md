

- Audio Toolbox
- AUAudioUnit
-  shouldChange(to:for:) 

Instance Method

# shouldChange(to:for:)

This is called when you set the format on a bus.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func shouldChange(
    to format: AVAudioFormat,
    for bus: AUAudioUnitBus
) -> Bool
```

## Parameters 

`format`  

The proposed new format.

`bus`  

The bus on which the format will be changed.

## Return Value

\- true if the new format will be set on the bus.

## Discussion

- false if the new format will not be set on the bus.

## Discussion

The bus has already checked that the format meets its channel constraints. The audio unit can override this method to check the format before allowing it to be set on the bus.

The default implementation returns false if the audio unit’s renderResourcesAllocated value is true.

## See Also

### Customizing the Audio Unit Behavior

class func registerSubclass(AnyClass, as: AudioComponentDescription, name: String, version: UInt32)

Registers an audio unit subclass.

func setRenderResourcesAllocated(Bool)

Sets the Boolean value of the renderResourcesAllocated property.

var internalRenderBlock: AUInternalRenderBlock

The block which you must provide, via a getter, in order to implement rendering.

var midiOutputBufferSizeHint: Int

typealias AUInternalRenderBlock

A block to render the audio unit.

