

- System
- FilePermissions
-  init(rawValue:) 

Initializer

# init(rawValue:)

Create a strongly-typed file permission from a raw C value.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(rawValue: CModeT)
```

## See Also

### Interacting with C APIs

let rawValue: CModeT

The raw C file permissions.

typealias CModeT

The C `mode_t` type.

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

