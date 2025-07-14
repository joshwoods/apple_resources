

- Swift Charts
- Plottable
-  init(primitivePlottable:) 

Initializer

# init(primitivePlottable:)

Creates the plottable value for the underlying type, if any, that corresponds to the primitive plottable value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init?(primitivePlottable: Self.PrimitivePlottable)
```

**Required** Default implementations provided.

## Discussion

This initializer fails if there is no corresponding plottable value.

## Default Implementations

### Plottable Implementations

init?(primitivePlottable: Self.PrimitivePlottable)

Creates the plottable value for the underlying type, if any, that corresponds to the primitive plottable value.

init?(primitivePlottable: Self.RawValue)

