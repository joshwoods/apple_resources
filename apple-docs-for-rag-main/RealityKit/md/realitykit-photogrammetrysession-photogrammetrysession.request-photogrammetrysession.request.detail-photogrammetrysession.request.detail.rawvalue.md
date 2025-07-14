

- RealityKit
- PhotogrammetrySession
- PhotogrammetrySession.Request
- PhotogrammetrySession.Request.Detail
-  PhotogrammetrySession.Request.Detail.RawValue 

Type Alias

# PhotogrammetrySession.Request.Detail.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 15.0+macOS 12.0+

``` source
typealias RawValue = Int
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Using enumeration raw values

var rawValue: Int

The corresponding value of the raw type.

init?(rawValue: Int)

Creates a new instance with the specified raw value.

