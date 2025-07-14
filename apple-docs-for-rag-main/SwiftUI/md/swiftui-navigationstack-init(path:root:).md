

- SwiftUI
- NavigationStack
-  init(path:root:) 

Initializer

# init(path:root:)

Creates a navigation stack with homogeneous navigation state that you can control.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(
    path: Binding,
    @ViewBuilder root: () -> Root
) where Data : MutableCollection, Data : RandomAccessCollection, Data : RangeReplaceableCollection, Data.Element : Hashable
```

Show all declarations

## Parameters 

`path`  

A Binding to the navigation state for this stack.

`root`  

The view to display when the stack is empty.

## Mentioned in 

Migrating to new navigation types

## Discussion

If you don’t need access to the navigation state, use init(root:).

