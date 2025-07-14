

- SwiftUI
- ForEach
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the identity of the underlying data.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
@MainActor
init(
    _ data: Data,
    @MapContentBuilder content: @escaping (Data.Element) -> Content
) where ID == Data.Element.ID, Data.Element : Identifiable
```

Available when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `MapContent`.

Show all declarations

## Parameters 

`data`  

The identified data that the ForEach instance uses to create map content dynamically.

`content`  

The map content builder that creates map content dynamically.

## Discussion

It’s important that the `id` of a data element doesn’t change unless you replace the data element with a new data element that has a new identity. If the `id` of a data element changes, the content view generated from that data element loses any current state and animations.

## See Also

### Creating a collection

init(Data)

Creates an instance that uniquely identifies and creates table rows across updates based on the identity of the underlying data.

init(_:id:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the provided key path to the underlying data’s identifier.

