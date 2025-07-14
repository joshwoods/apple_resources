

- DeveloperToolsSupport
- LibraryItem
-  LibraryItem.Category 

Structure

# LibraryItem.Category

The kinds of library items that you can create.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct Category
```

## Overview

When you specify a category for a library item, Xcode can group it with similar items in the library, making it easier for you to find. Categories provide visual treatment in the Xcode Library, but the treatment for each category depends on where the asset resides within the library.

## Topics

### Specifying a Category

static let control: LibraryItem.Category

A category for controls, like buttons and context menus.

static let effect: LibraryItem.Category

A category for effects, like opacity and saturation modifiers.

static let layout: LibraryItem.Category

A category for items that manage layout, like stack views and frame modifiers.

static let other: LibraryItem.Category

A general category.

## See Also

### Creating a Library Item

init&lt;SnippetExpressionType>(@autoclosure () -> SnippetExpressionType, visible: Bool, title: String?, category: LibraryItem.Category, matchingSignature: String?)

Creates a new library item.

