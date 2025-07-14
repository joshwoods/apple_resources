

- Core MIDI
- MIDIControlTransform
-  remappedControlType 

Instance Property

# remappedControlType

The remapped control type.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var remappedControlType: MIDITransformControlType
```

## Discussion

If transform is MIDITransformType.mapControl, the output control type.

## See Also

### Configuring a Control Transform

var controlType: MIDITransformControlType

The type of control specified by the control number.

var controlNumber: UInt16

The control number to affect.

var transform: MIDITransformType

The type of transformation to apply to the event values.

var param: Int16

An argument to the transformation method.

