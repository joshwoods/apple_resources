

- Core Haptics
- CHHapticPattern
-  init(events:parameters:) 

Initializer

# init(events:parameters:)

Constructs a haptic pattern from a series of events and parameters.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(
    events: [CHHapticEvent],
    parameters: [CHHapticDynamicParameter]
) throws
```

## Parameters 

`events`  

An array of events that make up the haptic pattern.

`parameters`  

An array of dynamic parameters that define how the haptic pattern’s parameters change over time.

## See Also

### Creating a Haptic Pattern

init(contentsOf: URL) throws

Creates a haptic pattern with the contents of an AHAP file.

init(events: [CHHapticEvent], parameterCurves: [CHHapticParameterCurve]) throws

Constructs a haptic pattern from a series of events and parameter curves.

init(dictionary: [CHHapticPattern.Key : Any]) throws

Creates a haptic pattern from a property list dictionary.

struct Key

Constants that define the keys you use to create a haptic pattern dictionary.

