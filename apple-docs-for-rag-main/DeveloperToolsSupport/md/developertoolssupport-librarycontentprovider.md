

- DeveloperToolsSupport
-  LibraryContentProvider 

Protocol

# LibraryContentProvider

A source of Xcode library and code completion content.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
protocol LibraryContentProvider
```

## Overview

Xcode discovers implementations of the `LibraryContentProvider` protocol in your project or workspace and examines their contents for items that it can add to the Xcode library. Add views by implementing the content provider’s computed views property, and returning an array of LibraryItem instances initialized with the views you want to publish:

```
```

Add view modifiers by implementing the modifiers(base:) method and similarly returning an array of library items initialized with the modifiers you want to publish. For view modifiers, you also specify the type to which the modifiers apply:

```
```

For modifiers that you define in an extension to View, you can provide any view conformer as the `base`. For modifiers that you define on a particular view type, provide that type as the `base`.

## Topics

### Adding Views

var views: [LibraryItem]

The SwiftUI views that you want to add to the Xcode library.

**Required** Default implementation provided.

### Adding Modifiers

func modifiers(base: Self.ModifierBase) -> [LibraryItem]

Indicates a collection of SwiftUI view modifiers to add to the Xcode library.

**Required** Default implementation provided.

associatedtype ModifierBase = Any

A type to use as a base for modifier completions.

**Required**

### Building Arrays

struct LibraryContentBuilder

A function builder for generating arrays of library items without requiring full array literal syntax.

## See Also

### Library Customization

struct LibraryItem

A single item to add to the Xcode library.

