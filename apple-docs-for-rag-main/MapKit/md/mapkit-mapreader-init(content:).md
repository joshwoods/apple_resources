

- MapKit
- MapReader
-  init(content:) 

Initializer

# init(content:)

Creates an instance that allows view content to reference information about a contained map.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(@ViewBuilder content: @escaping (MapProxy) -> Content)
```

## Parameters 

`content`  

The content of the map reader uses to retrieve information about, it uses the first map the `content` contains.

## Return Value

Returns a MapProxy that allows you to introspect the content of a map.

