

- DeveloperToolsSupport
-  LibraryContentBuilder 

Structure

# LibraryContentBuilder

A function builder for generating arrays of library items without requiring full array literal syntax.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@resultBuilder
struct LibraryContentBuilder
```

## Overview

Use the library content function builder to simplify the implementation of protocol requirements from you which provide arrays of library items. For example, without the builder, you would have to explicitly put items in an array in a views implementation:

```
struct LibraryViewContent: LibraryContentProvider {
    var views: [LibraryItem] {
        [
            LibraryItem(MyFirstView()),
            LibraryItem(MySecondView())
        ]
    }
}
```

With the builder, you can omit the array literal syntax:

```
struct LibraryViewContent: LibraryContentProvider {
    @LibraryContentBuilder
    var views: [LibraryItem] {
        LibraryItem(MyFirstView())
        LibraryItem(MySecondView())
    }
}
```

In practice, the Swift compiler infers the need for a library content builder attribute and adds it at build time, so that you never need to explicitly write the attribute in your code, even though it’s technically in use:

```
struct LibraryViewContent: LibraryContentProvider {
    var views: [LibraryItems] {
        LibraryItem(MyFirstView())
        LibraryItem(MySecondView())
    }
}
```

## Topics

### Type Methods

static func buildBlock([LibraryItem]...) -> [LibraryItem]

static func buildExpression(LibraryItem) -> [LibraryItem]

static func buildExpression([LibraryItem]) -> [LibraryItem]

