

- SwiftUI
-  TableRowBuilder 

Structure

# TableRowBuilder

A result builder that creates table row content from closures.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@resultBuilder
struct TableRowBuilder where Value : Identifiable
```

## Overview

The `buildBlock` methods in this type create TableRowContent instances based on the number and types of sources provided as parameters.

Don’t use this type directly; instead, SwiftUI annotates the `rows` parameter of the various Table initializers with the `@TableRowBuilder` annotation, implicitly calling this builder for you.

## Topics

### Building a row from sources

static func buildBlock&lt;C>(C) -> C

Creates a single row result.

static func buildBlock&lt;C0, C1>(C0, C1) -> TupleTableRowContent&lt;Value, (C0, C1)>

Creates a row result from two sources.

static func buildBlock&lt;C0, C1, C2>(C0, C1, C2) -> TupleTableRowContent&lt;Value, (C0, C1, C2)>

Creates a row result from three sources.

static func buildBlock&lt;C0, C1, C2, C3>(C0, C1, C2, C3) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3)>

Creates a row result from four sources.

static func buildBlock&lt;C0, C1, C2, C3, C4>(C0, C1, C2, C3, C4) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4)>

Creates a row result from five sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5>(C0, C1, C2, C3, C4, C5) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5)>

Creates a row result from six sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6>(C0, C1, C2, C3, C4, C5, C6) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6)>

Creates a row result from seven sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7>(C0, C1, C2, C3, C4, C5, C6, C7) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6, C7)>

Creates a row result from eight sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8>(C0, C1, C2, C3, C4, C5, C6, C7, C8) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8)>

Creates a row result from nine sources.

static func buildBlock&lt;C0, C1, C2, C3, C4, C5, C6, C7, C8, C9>(C0, C1, C2, C3, C4, C5, C6, C7, C8, C9) -> TupleTableRowContent&lt;Value, (C0, C1, C2, C3, C4, C5, C6, C7, C8, C9)>

Creates a row result from ten sources.

### Building a row from conditionals

static func buildIf&lt;C>(C?) -> C?

Creates a row result for conditional statements.

static func buildEither&lt;T, F>(first: T) -> _ConditionalContent&lt;T, F>

Creates a row result for the first of two row content alternatives.

static func buildEither&lt;T, F>(second: F) -> _ConditionalContent&lt;T, F>

Creates a row result for the second of two row content alternatives.

static func buildExpression&lt;Content>(Content) -> Content

Builds an expression within the builder.

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

protocol DynamicTableRowContent

A type of table row content that generates table rows from an underlying collection of data.

