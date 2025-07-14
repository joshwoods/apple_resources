

- MapKit
-  MapContentView 

Structure

# MapContentView

A view that contains content that displays on a map at a specific position, and that responds to specific interactions you specify.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
struct MapContentView where SelectionValue : Hashable, Content : MapContent
```

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Protocols

protocol DynamicMapContent

A  type of view that generates views from an underlying collection of data.

protocol MapContent

A protocol used to construct map content such as controls, markers, and annotations.

struct MapContentBuilder

A result builder that creates map content from closures you provide.

