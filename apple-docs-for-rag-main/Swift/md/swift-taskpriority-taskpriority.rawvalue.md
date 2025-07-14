

- Swift
- TaskPriority
-  TaskPriority.RawValue 

Type Alias

# TaskPriority.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
typealias RawValue = UInt8
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

