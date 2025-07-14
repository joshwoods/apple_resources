

- Audio Toolbox
- AUAudioUnitBusArray
-  init(audioUnit:busType:busses:) 

Initializer

# init(audioUnit:busType:busses:)

Initializes a bus array by making a copy of the supplied busses.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    audioUnit owner: AUAudioUnit,
    busType: AUAudioUnitBusType,
    busses busArray: [AUAudioUnitBus]
)
```

## Parameters 

`owner`  

The audio unit that owns the bus array.

`busType`  

Determines whether the busses are for input or output.

`busArray`  

An array of busses.

## Return Value

A newly-initialized bus array.

## See Also

### Initialization

convenience init(audioUnit: AUAudioUnit, busType: AUAudioUnitBusType)

Initializes an empty bus array.

