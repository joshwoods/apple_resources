

- Audio Toolbox
- AUAudioUnitBusArray
-  init(audioUnit:busType:) 

Initializer

# init(audioUnit:busType:)

Initializes an empty bus array.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    audioUnit owner: AUAudioUnit,
    busType: AUAudioUnitBusType
)
```

## Parameters 

`owner`  

The audio unit that owns the bus array.

`busType`  

Determines whether the bus array is for input or output.

## Return Value

A newly-initialized bus array.

## See Also

### Initialization

init(audioUnit: AUAudioUnit, busType: AUAudioUnitBusType, busses: [AUAudioUnitBus])

Initializes a bus array by making a copy of the supplied busses.

