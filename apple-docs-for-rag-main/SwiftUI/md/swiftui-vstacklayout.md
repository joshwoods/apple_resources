

- SwiftUI
-  VStackLayout 

Structure

# VStackLayout

A vertical container that you can use in conditional layouts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct VStackLayout
```

## Overview

This layout container behaves like a VStack, but conforms to the Layout protocol so you can use it in the conditional layouts that you construct with AnyLayout. If you don’t need a conditional layout, use VStack instead.

## Topics

### Creating a vertical stack

init(alignment: HorizontalAlignment, spacing: CGFloat?)

Creates a vertical stack with the specified spacing and horizontal alignment.

### Getting the stack’s properties

var alignment: HorizontalAlignment

The horizontal alignment of subviews.

var spacing: CGFloat?

The distance between adjacent subviews.

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

struct ZStackLayout

An overlaying container that you can use in conditional layouts.

struct GridLayout

A grid that you can use in conditional layouts.

