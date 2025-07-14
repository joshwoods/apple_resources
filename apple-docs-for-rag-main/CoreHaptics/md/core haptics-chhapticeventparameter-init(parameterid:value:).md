

- Core Haptics
- CHHapticEventParameter
-  init(parameterID:value:) 

Initializer

# init(parameterID:value:)

Creates a haptic event parameter from its ID and value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    parameterID: CHHapticEvent.ParameterID,
    value: Float
)
```

## Parameters 

`parameterID`  

The ID indicating the type of the event parameter.

`value`  

The value of the event parameter.

## See Also

### Creating an Event Parameter

struct ParameterID

An identifier for an event parameter.

