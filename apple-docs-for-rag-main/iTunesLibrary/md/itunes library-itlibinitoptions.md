

- iTunes Library
-  ITLibInitOptions 

Enumeration

# ITLibInitOptions

These constants describe initialization options for an iTunes library.

Mac Catalyst 14.0+macOS 10.13+

``` source
enum ITLibInitOptions
```

## Topics

### Init Options

case none

No initialization options apply.

case lazyLoadData

iTunes library data loads upon request, rather than during initialization.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Essentials

convenience init(apiVersion: String) throws

Initializes an instance of ITLibrary that can retrieve media entities.

init(apiVersion: String, options: ITLibInitOptions) throws

Initializes an instance of `ITLibrary` that can retrieve media entities.

