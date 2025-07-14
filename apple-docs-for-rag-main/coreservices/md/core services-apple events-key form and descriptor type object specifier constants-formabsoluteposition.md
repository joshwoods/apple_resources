

- Core Services
- Apple Events
- Key Form and Descriptor Type Object Specifier Constants
-  formAbsolutePosition 

Global Variable

# formAbsolutePosition

Mac Catalyst 13.0+macOS 10.0+

``` source
var formAbsolutePosition: Int { get }
```

## Discussion

An integer or other constant indicating the position of one or more elements in relation to the beginning or end of their container. The key data consists of an integer that specifies either an offset or an ordinal position.

For descriptor type `typeAbsoluteOrdinal`, the data consists of one of the constants `kAEFirst`, `kAEMiddle`, `kAELast`, `kAEAny`, or `kAEAll`, which are described in AEDisposeToken(_:).

For other descriptor types, the data can be coerced to either a positive integer, indicating the offset of the requested element from the beginning of the container, or a negative integer, indicating its offset from the end of the container.

