

- Core Services
- Carbon Core
- Unicode Utilities
-  CollatorRef 

Type Alias

# CollatorRef

Refers to an opaque object that encapsulates locale and collation information for the purpose of performing Unicode string comparison.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias CollatorRef = OpaquePointer
```

## Discussion

You can obtain a `CollatorRef` value from the function UCCreateCollator(_:_:_:_:).

