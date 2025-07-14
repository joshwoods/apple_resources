

- SwiftUI
- TableColumnForEach
-  init(\_:id:content:) 

Initializer

# init(\_:id:content:)

Creates an instance that uniquely identifies and creates table columns across updates based on the provided key path to the underlying data’s identifier.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+macOS 14.4+visionOS 1.1+

``` source
init(
    _ data: Data,
    id: KeyPath,
    @TableColumnBuilder.TableRowValue, TableColumnForEach.TableColumnSortComparator> content: @escaping (Data.Element) -> Content
)
```

## Parameters 

`data`  

The data that the TableColumnForEach instance uses to create table columns dynamically.

`id`  

The key path to the provided data’s identifier.

`content`  

The table column builder that creates columns dynamically for each element.

## See Also

### Creating the collection

init(_:content:)

Creates an instance that uniquely identifies and creates table columns across updates based on the identity of the underlying data.

