

- SwiftUI
-  TableOutlineGroupContent 

Structure

# TableOutlineGroupContent

An opaque table row type created by a table’s hierarchical initializers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct TableOutlineGroupContent where Data : RandomAccessCollection, Data.Element : Identifiable
```

## Overview

This row content is created by `Table.init(_:,children:,...)` initializers as the table’s `Rows` generic type.

To explicitly create hierarchical rows, use OutlineGroup instead.

## Relationships

### Conforms To

- TableRowContent

## See Also

### Adding progressive disclosure

struct DisclosureTableRow

A kind of table row that shows or hides additional rows based on the state of a disclosure control.

