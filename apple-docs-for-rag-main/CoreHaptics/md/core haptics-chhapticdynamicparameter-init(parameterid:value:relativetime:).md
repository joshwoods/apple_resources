

- Core Haptics
- CHHapticDynamicParameter
-  init(parameterID:value:relativeTime:) 

Initializer

# init(parameterID:value:relativeTime:)

Creates a dynamic parameter from its ID, value, and start time.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    parameterID: CHHapticDynamicParameter.ID,
    value: Float,
    relativeTime time: TimeInterval
)
```

## Parameters 

`parameterID`  

The ID indicating the type of the dynamic parameter.

`value`  

The value of the dynamic parameter.

`time`  

The time at which to send the dynamic parameter.

## See Also

### Creating a Dynamic Parameter

struct ID

The identifier that reveals the type of property associated with a dynamic parameter.

