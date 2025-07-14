

- AVFAudio
- AVParameterEvent
-  init(parameterID:scope:element:value:) 

Initializer

# init(parameterID:scope:element:value:)

Creates an event with a parameter identifier, scope, element, and value for the parameter to set.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(
    parameterID: UInt32,
    scope: UInt32,
    element: UInt32,
    value: Float
)
```

## Parameters 

`parameterID`  

The identifier of the parameter.

`scope`  

The audio unit scope for the parameter.

`element`  

The element index in the scope.

`value`  

The value of the parameter to set.

## Discussion

For more information about the parameters, see AudioUnitParameterID, AudioUnitScope, and AudioUnitElement. The valid range of values depend on the parameter you set.

