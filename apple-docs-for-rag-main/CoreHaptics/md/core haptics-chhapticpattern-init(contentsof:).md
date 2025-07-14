

- Core Haptics
- CHHapticPattern
-  init(contentsOf:) 

Initializer

# init(contentsOf:)

Creates a haptic pattern with the contents of an AHAP file.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
init(contentsOf ahapURL: URL) throws
```

## Parameters 

`ahapURL`  

A URL to an AHAP file that describes a pattern.

## See Also

### Creating a Haptic Pattern

init(events: [CHHapticEvent], parameterCurves: [CHHapticParameterCurve]) throws

Constructs a haptic pattern from a series of events and parameter curves.

init(events: [CHHapticEvent], parameters: [CHHapticDynamicParameter]) throws

Constructs a haptic pattern from a series of events and parameters.

init(dictionary: [CHHapticPattern.Key : Any]) throws

Creates a haptic pattern from a property list dictionary.

struct Key

Constants that define the keys you use to create a haptic pattern dictionary.

