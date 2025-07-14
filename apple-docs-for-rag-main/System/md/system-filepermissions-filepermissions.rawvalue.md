

- System
- FilePermissions
-  FilePermissions.RawValue 

Type Alias

# FilePermissions.RawValue

The raw type that can be used to represent all values of the conforming type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
typealias RawValue = CModeT
```

## Discussion

Every distinct value of the conforming type has a corresponding unique value of the `RawValue` type, but there may be values of the `RawValue` type that don’t have a corresponding value of the conforming type.

## See Also

### Interacting with C APIs

init(rawValue: CModeT)

Create a strongly-typed file permission from a raw C value.

let rawValue: CModeT

The raw C file permissions.

typealias CModeT

The C `mode_t` type.

