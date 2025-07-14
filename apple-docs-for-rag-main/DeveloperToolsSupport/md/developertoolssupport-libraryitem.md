

- DeveloperToolsSupport
-  LibraryItem 

Structure

# LibraryItem

A single item to add to the Xcode library.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct LibraryItem
```

## Overview

Declare a library item to describe an entry in the Xcode library. Xcode discovers and validates library items that you place in the context of a LibraryContentProvider instance.

At a minimum, you provide an expression that Xcode uses when the user chooses the library item. You can provide any expression that compiles in the context of the library item instantiation. However, Xcode only honors items that adhere to certain restrictions, as described in views and modifiers(base:).

You can also provide additional characteristics, like a title and a category, to help you find the item when searching the library.

## Topics

### Creating a Library Item

init&lt;SnippetExpressionType>(@autoclosure () -> SnippetExpressionType, visible: Bool, title: String?, category: LibraryItem.Category, matchingSignature: String?)

Creates a new library item.

struct Category

The kinds of library items that you can create.

## See Also

### Library Customization

protocol LibraryContentProvider

A source of Xcode library and code completion content.

