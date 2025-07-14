

- SwiftUI
- ForEach
-  init(\_:id:content:) 

Initializer

# init(\_:id:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the provided key path to the underlying data’s identifier.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
@MainActor
init(
    _ data: Data,
    id: KeyPath,
    @MapContentBuilder content: @escaping (Data.Element) -> Content
)
```

Available when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `MapContent`.

Show all declarations

## Parameters 

`data`  

The data that the ForEach instance uses to create map content dynamically.

`id`  

The key path to the provided data’s identifier.

`content`  

The map content builder that creates map content dynamically.

## Mentioned in 

Creating performant scrollable stacks

## Discussion

It’s important that the `id` of a data element doesn’t change, unless the data element has been replaced with a new data element that has a new identity. If the `id` of a data element changes, then the map content generated from that data element will lose any current state and animations.

## See Also

### Creating a collection

init(Data)

Creates an instance that uniquely identifies and creates table rows across updates based on the identity of the underlying data.

init(_:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the identity of the underlying data.

