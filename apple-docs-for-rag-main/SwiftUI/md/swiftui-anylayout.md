

- SwiftUI
-  AnyLayout 

Structure

# AnyLayout

A type-erased instance of the layout protocol.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct AnyLayout
```

## Overview

Use an `AnyLayout` instance to enable dynamically changing the type of a layout container without destroying the state of the subviews. For example, you can create a layout that changes between horizontal and vertical layouts based on the current Dynamic Type setting:

```
struct DynamicLayoutExample: View {
    @Environment(\.dynamicTypeSize) var dynamicTypeSize

    var body: some View {
        let layout = dynamicTypeSize 

The types that you use with `AnyLayout` must conform to the Layout protocol. The above example chooses between the HStackLayout and VStackLayout types, which are versions of the built-in HStack and VStack containers that conform to the protocol. You can also use custom layout types that you define.

## Topics

### Creating the layout

init&lt;L>(L)

Creates a type-erased value that wraps the specified layout.

## Relationships

### Conforms To

- Animatable
- Layout

## See Also

### Transitioning between layout types

struct HStackLayout

A horizontal container that you can use in conditional layouts.

struct VStackLayout

A vertical container that you can use in conditional layouts.

struct ZStackLayout

An overlaying container that you can use in conditional layouts.

struct GridLayout

A grid that you can use in conditional layouts.

