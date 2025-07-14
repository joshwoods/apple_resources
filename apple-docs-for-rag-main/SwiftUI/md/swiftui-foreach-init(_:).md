

- SwiftUI
- ForEach
-  init(\_:) 

Initializer

# init(\_:)

Creates an instance that uniquely identifies and creates table rows across updates based on the identity of the underlying data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(_ data: Data) where ID == Data.Element.ID, Content == TableRow, Data.Element : Identifiable
```

Available when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TableRowContent`.

## Parameters 

`data`  

The identified data that the ForEach instance uses to create table rows dynamically.

## Discussion

The following example creates a `Person` type that conforms to Identifiable, and an array of this type called `people`. A `ForEach` instance iterates over the array, producing new TableRow instances implicitly.

```
private struct Person: Identifiable {
    var id = UUID()
    var name: String
}

@State private var people: [Person] = /* ... */

Table(of: Person.self) {
    TableColumn("ID", value: \.id.uuidString)
    TableColumn("Name", value: \.name)
} rows: {
    Section("Team") {
        /* This is equivalent to the line below:
        ForEach(people) { TableRow($0) }
        */
        ForEach(people)
    }
}
```

## See Also

### Creating a collection

init(_:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the identity of the underlying data.

init(_:id:content:)

Creates an instance that uniquely identifies and creates map content across updates based on the provided key path to the underlying data’s identifier.

