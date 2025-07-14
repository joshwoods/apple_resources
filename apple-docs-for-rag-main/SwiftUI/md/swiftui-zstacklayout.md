

- SwiftUI
-  ZStackLayout 

Structure

# ZStackLayout

An overlaying container that you can use in conditional layouts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct ZStackLayout
```

## Overview

This layout container behaves like a ZStack, but conforms to the Layout protocol so you can use it in the conditional layouts that you construct with AnyLayout. If you don’t need a conditional layout, use ZStack instead.

## Topics

### Creating a stack

init(alignment: Alignment)

Creates a stack with the specified alignment.

### Getting the stack’s properties

var alignment: Alignment

The alignment of subviews.

## Relationships

### Conforms To

- Animatable
- BitwiseCopyable
- Copyable
- Layout
- Sendable

## See Also

### Transitioning between layout types

struct AnyLayout

A type-erased instance of the layout protocol.

struct HStackLayout

A horizontal container that you can use in conditional layouts.

struct VStackLayout

A vertical container that you can use in conditional layouts.

struct GridLayout

A grid that you can use in conditional layouts.

