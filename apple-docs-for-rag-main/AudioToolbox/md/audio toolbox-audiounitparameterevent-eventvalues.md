

- Audio Toolbox
- AudioUnitParameterEvent
-  eventValues 

Instance Property

# eventValues

The values for this parameter event.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var eventValues: AudioUnitParameterEvent.__Unnamed_union_eventValues
```

## Discussion

If the parameter event type is AUParameterEventType.parameterEvent_Immediate, use the `immediate` struct of this union. If the parameter event type is AUParameterEventType.parameterEvent_Ramped, use the `ramp` struct of this union.

#### immediate

**bufferOffset**  
A `UInt32` value that indicates the sample time at which to change the parameter value.

**value**  
An AudioUnitParameterValue that indicates the new parameter value.

#### ramp

**startBufferOffset**  
An `SInt32` value that indicates the sample time at which to begin the parameter value change.

**durationInFrames**  
A `UInt32` value that indicates the number of frames over which the parameter value should linearly change from `startValue` to `endValue`.

**startValue**  
An AudioUnitParameterValue that indicates the starting parameter value.

**endValue**  
An AudioUnitParameterValue that indicates the ending parameter value.

## See Also

### Fields

var scope: AudioUnitScope

The scope for this parameter event.

var element: AudioUnitElement

The element for this parameter event.

var parameter: AudioUnitParameterID

An identifier for this parameter event.

var eventType: AUParameterEventType

The type for this parameter event.

