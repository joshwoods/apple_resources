

- SwiftUI
-  ToolbarContent 

Protocol

# ToolbarContent

Conforming types represent items that can be placed in various locations in a toolbar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
protocol ToolbarContent
```

## Overview

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

### Implementing toolbar content

var body: Self.Body

The composition of content that comprise the toolbar content.

**Required**

associatedtype Body : ToolbarContent

The type of content representing the body of this toolbar content.

**Required**

### Instance Methods

func hidden(Bool) -> some ToolbarContent

Hides a toolbar item within its toolbar.

## Relationships

### Inherited By

- CustomizableToolbarContent

### Conforming Types

- Group

  Conforms when `Content` conforms to `CustomizableToolbarContent`.

- ToolbarItem
- ToolbarItemGroup
- ToolbarTitleMenu

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

struct ToolbarContentBuilder

Constructs a toolbar item set from multi-expression closures.

