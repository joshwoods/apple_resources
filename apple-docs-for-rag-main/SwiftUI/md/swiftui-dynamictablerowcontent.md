

- SwiftUI
-  DynamicTableRowContent 

Protocol

# DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
protocol DynamicTableRowContent : TableRowContent
```

## Overview

This table row content type provides drag-and-drop support for tables. Use the onInsert(of:perform:) modifier to add an action to call when the table inserts new contents into its underlying collection.

## Topics

### Getting row data

var data: Self.Data

The collection of underlying data.

**Required**

associatedtype Data : Collection

The type of the underlying collection of data.

**Required**

### Inserting rows

func onInsert(of: [UTType], perform: (Int, [NSItemProvider]) -> Void) -> ModifiedContent&lt;Self, OnInsertTableRowModifier>

Sets the insert action for the dynamic table rows.

struct OnInsertTableRowModifier

A table row modifier that adds the ability to insert data in some base row content.

### Supporting drag and drop

func dropDestination&lt;T>(for: T.Type, action: (Int, [T]) -> Void) -> ModifiedContent&lt;Self, OnInsertTableRowModifier>

Sets the insert action for the dynamic table rows.

## Relationships

### Inherits From

- TableRowContent

### Conforming Types

- ForEach

  Conforms when `Data` conforms to `RandomAccessCollection`, `ID` conforms to `Hashable`, and `Content` conforms to `TableRowContent`.

- ModifiedContent

  Conforms when `Content` conforms to `DynamicTableRowContent` and `Modifier` conforms to `_TableRowContentModifier`.

## See Also

### Creating rows

struct TableRow

A row that represents a data value in a table.

protocol TableRowContent

A type used to represent table rows.

struct TableHeaderRowContent

A table row that displays a single view instead of columned content.

struct TupleTableRowContent

A type of table column content that creates table rows created from a Swift tuple of table rows.

struct TableForEachContent

A type of table row content that creates table rows created by iterating over a collection.

struct EmptyTableRowContent

A table row content that doesn’t produce any rows.

struct TableRowBuilder

A result builder that creates table row content from closures.

