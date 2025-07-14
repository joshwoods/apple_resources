

- RealityKit
- ModelDebugOptionsComponent
- ModelDebugOptionsComponent.VisualizationMode
-  ModelDebugOptionsComponent.VisualizationMode.RawValue 

Type Alias

# ModelDebugOptionsComponent.VisualizationMode.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Raw values

init?(rawValue: String)

Creates a new instance with the specified raw value.

var rawValue: String

The corresponding value of the raw type.

