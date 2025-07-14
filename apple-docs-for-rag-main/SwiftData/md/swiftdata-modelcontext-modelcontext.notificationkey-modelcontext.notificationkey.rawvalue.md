

- SwiftData
- ModelContext
- ModelContext.NotificationKey
-  ModelContext.NotificationKey.RawValue 

Type Alias

# ModelContext.NotificationKey.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+Swift 5.9+

``` source
typealias RawValue = String
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

