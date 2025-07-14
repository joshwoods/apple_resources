

- Core Haptics
- CHHapticPattern
-  init(dictionary:) 

Initializer

# init(dictionary:)

Creates a haptic pattern from a property list dictionary.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 14.0+visionOS 1.0+

``` source
init(dictionary patternDict: [CHHapticPattern.Key : Any]) throws
```

## Parameters 

`patternDict`  

A dictionary that defines the haptic pattern and its parameters.

## See Also

### Creating a Haptic Pattern

init(contentsOf: URL) throws

Creates a haptic pattern with the contents of an AHAP file.

init(events: [CHHapticEvent], parameterCurves: [CHHapticParameterCurve]) throws

Constructs a haptic pattern from a series of events and parameter curves.

init(events: [CHHapticEvent], parameters: [CHHapticDynamicParameter]) throws

Constructs a haptic pattern from a series of events and parameters.

struct Key

Constants that define the keys you use to create a haptic pattern dictionary.

