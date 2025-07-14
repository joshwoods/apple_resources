

- SwiftUI
-  ToolbarContentBuilder 

Structure

# ToolbarContentBuilder

Constructs a toolbar item set from multi-expression closures.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@resultBuilder
struct ToolbarContentBuilder
```

## Topics

### Building toolbar content

static buildBlock(_:)

static buildBlock(_:_:)

static buildBlock(_:_:_:)

static buildBlock(_:_:_:_:)

static buildBlock(_:_:_:_:_:)

static buildBlock(_:_:_:_:_:_:)

static buildBlock(_:_:_:_:_:_:_:)

static buildBlock(_:_:_:_:_:_:_:_:)

static buildBlock(_:_:_:_:_:_:_:_:_:)

static buildBlock(_:_:_:_:_:_:_:_:_:_:)

### Building conditional toolbar content

static buildIf(_:)

static buildEither(first:)

static buildEither(second:)

static buildExpression(_:)

Builds an expression within the builder.

static buildLimitedAvailability(_:)

## See Also

### Populating a toolbar

func toolbar(content:)

Populates the toolbar or navigation bar with the specified items.

struct ToolbarItem

A model that represents an item which can be placed in the toolbar or navigation bar.

struct ToolbarItemGroup

A model that represents a group of `ToolbarItem`s which can be placed in the toolbar or navigation bar.

struct ToolbarItemPlacement

A structure that defines the placement of a toolbar item.

protocol ToolbarContent

Conforming types represent items that can be placed in various locations in a toolbar.

