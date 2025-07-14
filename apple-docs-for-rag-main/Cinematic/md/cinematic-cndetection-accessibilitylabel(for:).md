

- Cinematic
- CNDetection
-  accessibilityLabel(for:) 

Type Method

# accessibilityLabel(for:)

A localized accessibility label converting a specific detection type into a broad category such as a person, pet, and so on.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
static func accessibilityLabel(for detectionType: CNDetectionType) -> String
```

## Parameters 

`detectionType`  

The type of object to detect, such as the face, torso, cat, dog, and so on.

## Return Value

A string representing a localized accessibility label converting a specific detection type into a broad category such as a person, pet, and so on.

