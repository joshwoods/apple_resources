

- Core Services
- Carbon Core
- Unicode Utilities
-  TextBreakLocatorRef 

Type Alias

# TextBreakLocatorRef

Refers to an opaque object that encapsulates locale and text-break information for the purpose of finding boundaries in Unicode text.

Mac Catalyst 13.0+macOS 10.0+

``` source
typealias TextBreakLocatorRef = OpaquePointer
```

## Discussion

You can obtain a `TextBreakLocatorRef` value from the function UCCreateTextBreakLocator.

