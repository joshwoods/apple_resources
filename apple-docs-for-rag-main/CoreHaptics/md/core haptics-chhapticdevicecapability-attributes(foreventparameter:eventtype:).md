

- Core Haptics
- CHHapticDeviceCapability
-  attributes(forEventParameter:eventType:) 

Instance Method

# attributes(forEventParameter:eventType:)

Returns the haptic device’s attributes for an event parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
func attributes(
    forEventParameter inParameter: CHHapticEvent.ParameterID,
    eventType type: CHHapticEvent.EventType
) throws -> any CHHapticParameterAttributes
```

**Required**

## Parameters 

`inParameter`  

The event parameter ID whose attributes you seek.

`type`  

A haptic event type to query.

## Return Value

The haptic device’s attributes for the given event parameter ID.

## See Also

### Determining Supported Parameters

func attributes(forDynamicParameter: CHHapticDynamicParameter.ID) throws -> any CHHapticParameterAttributes

Requests the haptic device’s attributes for a dynamic parameter.

**Required**

