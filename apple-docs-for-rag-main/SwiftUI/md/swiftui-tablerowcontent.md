

- SwiftUI
-  TableRowContent 

Protocol

# TableRowContent

A type used to represent table rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol TableRowContent
```

## Overview

Like with the View protocol, you can create custom table row content by declaring a type that conforms to the `TableRowContent` protocol and implementing the required tableRowBody property.

```
struct GroupOfPeopleRows: TableRowContent {
    @Binding var people: [Person]

    var tableRowBody: some TableRowContent {
        ForEach(people) { person in
            TableRow(person)
                .itemProvider { person.itemProvider }
        }
        .dropDestination(for: Person.self) { destination, newPeople in
            people.insert(contentsOf: newPeople, at: destination)
        }
    }
}
```

This example uses an opaque result type and specifies that the primary associated type `TableRowValue` for the `tableRowBody` property is a `Person`. From this, SwiftUI can infer `TableRowValue` for the `GroupOfPeopleRows` structure is also `Person`.

A type conforming to this protocol inherits `@preconcurrency @MainActor` isolation from the protocol if the conformance is included in the type’s base declaration:

```
struct MyCustomType: Transition {
    // `@preconcurrency @MainActor` isolation by default
}
```

Isolation to the main actor is the default, but it’s not required. Declare the conformance in an extension to opt out of main actor isolation:

```
extension MyCustomType: Transition {
    // `nonisolated` by default
}
```

## Topics

### Getting the row body

var tableRowBody: Self.TableRowBody

The composition of content that comprise the table row content.

**Required**

associatedtype TableRowBody : TableRowContent

The type of content representing the body of this table row content.

**Required**

### Defining the row value

associatedtype TableRowValue : Identifiable = Self.TableRowBody.TableRowValue

The type of value represented by this table row content.

**Required**

### Managing interaction

func draggable&lt;T>(@autoclosure () -> T) -> some TableRowContent&lt;Self.TableRowValue> 

Activates this row as the source of a drag and drop operation.

func dropDestination&lt;T>(for: T.Type, action: ([T]) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Defines the entire row as a destination of a drag and drop operation that handles the dropped content with a closure that you specify.

func onHover(perform: (Bool) -> Void) -> some TableRowContent&lt;Self.TableRowValue> 

Adds an action to perform when the pointer moves onto or away from the entire row.

func itemProvider((() -> NSItemProvider?)?) -> ModifiedContent&lt;Self, ItemProviderTableRowModifier>

Provides a closure that vends the drag representation for a particular data element.

struct ItemProviderTableRowModifier

A table row modifier that associates an item provider with some base row content.

### Adding a context menu to a row

func contextMenu&lt;M>(menuItems: () -> M) -> ModifiedContent&lt;Self, _ContextMenuTableRowModifier&lt;M>>

Adds a context menu to a table row.

func contextMenu&lt;M, P>(menuItems: () -> M, preview: () -> P) -> ModifiedContent&lt;Self, _ContextMenuPreviewTableRowModifier&lt;M, P>>

Adds a context menu with a preview to a table row.

### Instance Methods

func selectionDisabled(Bool) -> some TableRowContent&lt;Self.TableRowValue> 

Adds a condition that controls whether users can select this row.

## Relationships

### Inherited By

- DynamicTableRowContent

### Conforming Types

- DisclosureTableRow
- EmptyTableRowContent

  Conforms when `Value` conforms to `Identifiable`.

- ForEach

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TableRowContent`.

- Group

  Conforms when `Content` conforms to `TableRowContent`.

- ModifiedContent

  Conforms when `Content` conforms to `DynamicTableRowContent` and `Modifier` conforms to `_TableRowContentModifier`.

- OutlineGroup

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` is `Data.Element.ID`, `Parent` conforms to `TableRowContent`, `Parent` is `Leaf`, `Leaf` is `Subgroup`, and `Data.Element` is `Parent.TableRowValue`.

- Section

  Conforms when `Parent` conforms to `TableRowContent`, `Content` conforms to `TableRowContent`, and `Footer` conforms to `TableRowContent`.

- TableForEachContent
- TableHeaderRowContent
- TableOutlineGroupContent
- TableRow
- TupleTableRowContent

## See Also

### Creating rows

struct TableRow

A row that represents a data value in a table.

struct TableHeaderRowContent

A table row that displays a single view instead of columned content.

struct TupleTableRowContent

A type of table column content that creates table rows created from a Swift tuple of table rows.

struct TableForEachContent

A type of table row content that creates table rows created by iterating over a collection.

struct EmptyTableRowContent

A table row content that doesn’t produce any rows.

protocol DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

struct TableRowBuilder

A result builder that creates table row content from closures.

