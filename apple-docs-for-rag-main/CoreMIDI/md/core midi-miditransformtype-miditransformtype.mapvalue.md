

- Core MIDI
- MIDITransformType
-  MIDITransformType.mapValue 

Case

# MIDITransformType.mapValue

A transform that maps one value to another.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
case mapValue
```

## Discussion

The value you specify is the index of the map in the connection’s array of maps.

## See Also

### Transform Types

case none

No transformation.

case filterOut

A transformation that filters out an event type.

case mapControl

A transformation that changes a specified control number to a supplied parameter value.

case add

A transform that adds a parameter value.

case scale

A transform that multiplies by the specified parameter value.

case minValue

A transform that sets the minimum value to the specified parameter value.

case maxValue

A transform that sets the maximum value to the specified parameter value.

