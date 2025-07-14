

- SwiftUI
-  TableColumnAlignment 

Structure

# TableColumnAlignment

Describes the alignment of the content of a table column.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
struct TableColumnAlignment
```

## Overview

The alignment of a column applies to both its header label as well as the default alignment of its content view for each row.

## Topics

### Getting the alignment

static var automatic: TableColumnAlignment

The default column alignment.

static var leading: TableColumnAlignment

Leading column alignment.

static var center: TableColumnAlignment

Center column alignment.

static var trailing: TableColumnAlignment

Trailing column alignment.

static var numeric: TableColumnAlignment

Column alignment appropriate for numeric content.

static func numeric(Locale.NumberingSystem) -> TableColumnAlignment

Column alignment appropriate for numeric content.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Creating columns

struct TableColumn

A column that displays a view for each row in a table.

protocol TableColumnContent

A type used to represent columns within a table.

struct TableColumnBuilder

A result builder that creates table column content from closures.

struct TableColumnForEach

A structure that computes columns on demand from an underlying collection of identified data.

