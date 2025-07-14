

- SwiftUI
-  TableStyle 

Protocol

# TableStyle

A type that applies a custom appearance to all tables within a view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
protocol TableStyle
```

## Overview

To configure the current table style for a view hierarchy, use the tableStyle(_:) modifier.

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

### Getting built-in table styles

static var automatic: AutomaticTableStyle

The default table style in the current context.

static var inset: InsetTableStyle

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

static var bordered: BorderedTableStyle

The table style that describes the behavior and appearance of a table with standard border.

### Creating custom table styles

func makeBody(configuration: Self.Configuration) -> Self.Body

Creates a view that represents the body of a table.

**Required**

typealias Configuration

The properties of a table.

associatedtype Body : View

A view that represents the body of a table.

**Required**

### Deprecated styles

static func inset(alternatesRowBackgrounds: Bool) -> InsetTableStyle

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

Deprecated

static func bordered(alternatesRowBackgrounds: Bool) -> BorderedTableStyle

The table style that describes the behavior and appearance of a table with standard border.

Deprecated

### Supporting types

struct AutomaticTableStyle

The default table style in the current context.

struct InsetTableStyle

The table style that describes the behavior and appearance of a table with its content and selection inset from the table edges.

struct BorderedTableStyle

The table style that describes the behavior and appearance of a table with standard border.

## Relationships

### Conforming Types

- AutomaticTableStyle
- BorderedTableStyle
- InsetTableStyle

## See Also

### Styling collection views

func listStyle&lt;S>(S) -> some View

Sets the style for lists within this view.

protocol ListStyle

A protocol that describes the behavior and appearance of a list.

func tableStyle&lt;S>(S) -> some View

Sets the style for tables within this view.

struct TableStyleConfiguration

The properties of a table.

func disclosureGroupStyle&lt;S>(S) -> some View

Sets the style for disclosure groups within this view.

protocol DisclosureGroupStyle

A type that specifies the appearance and interaction of disclosure groups within a view hierarchy.

