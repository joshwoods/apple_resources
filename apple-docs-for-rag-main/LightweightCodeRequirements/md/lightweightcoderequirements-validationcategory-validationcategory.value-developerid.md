

- LightweightCodeRequirements
- ValidationCategory
- ValidationCategory.Value
-  developerID 

Type Property

# developerID

Indicates that the code is signed by an Apple issued Developer ID certificate.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+tvOS 17.4+visionOS 1.1+watchOS 10.4+

``` source
static let developerID: ValidationCategory.Value
```

## Discussion

This category will only match process on macOS. This category could match code on disk on iOS/watchOS/tvOS/visionOS but that code cannot run.

