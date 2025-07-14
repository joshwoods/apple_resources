

- SwiftUI
- TableColumnForEach
-  init(\_:content:) 

Initializer

# init(\_:content:)

Creates an instance that uniquely identifies and creates table columns across updates based on the identity of the underlying data.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+visionOS 1.1+

``` source
init(
    _ data: Data,
    @TableColumnBuilder.TableRowValue, TableColumnForEach.TableColumnSortComparator> content: @escaping (Data.Element) -> Content
) where ID == Data.Element.ID, Data.Element : Identifiable
```

Show all declarations

## Parameters 

`data`  

The identified data that the TableColumnForEach instance uses to create table columns dynamically.

`content`  

The table column builder that creates columns dynamically for each element.

## See Also

### Creating the collection

init(Data, id: KeyPath&lt;Data.Element, ID>, content: (Data.Element) -> Content)

Creates an instance that uniquely identifies and creates table columns across updates based on the provided key path to the underlying data’s identifier.

