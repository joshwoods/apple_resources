

- DeveloperToolsSupport
- LibraryContentProvider
-  ModifierBase 

Associated Type

# ModifierBase

A type to use as a base for modifier completions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
associatedtype ModifierBase = Any
```

**Required**

## Discussion

To verify that the completion for a modifier compiles, you specify modifiers as they apply to some base type. Since most modifiers can modify any SwiftUI view, you typically specify any concrete implementation of the View protocol for `ModifierBase`. However, some modifiers apply to more specific types, like Image or Text, or to an entirely different type like Shape.

## See Also

### Adding Modifiers

func modifiers(base: Self.ModifierBase) -> [LibraryItem]

Indicates a collection of SwiftUI view modifiers to add to the Xcode library.

**Required** Default implementation provided.

