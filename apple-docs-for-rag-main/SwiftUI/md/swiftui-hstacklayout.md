

- SwiftUI
-  HStackLayout 

Structure

# HStackLayout

A horizontal container that you can use in conditional layouts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct HStackLayout
```

## Overview

This layout container behaves like an HStack, but conforms to the Layout protocol so you can use it in the conditional layouts that you construct with AnyLayout. If you don’t need a conditional layout, use HStack instead.

## Topics

### Creating a horizontal stack

init(alignment: VerticalAlignment, spacing: CGFloat?)

Creates a horizontal stack with the specified spacing and vertical alignment.

### Getting the stack’s properties

var alignment: VerticalAlignment

The vertical alignment of subviews.

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

struct VStackLayout

A vertical container that you can use in conditional layouts.

struct ZStackLayout

An overlaying container that you can use in conditional layouts.

struct GridLayout

A grid that you can use in conditional layouts.

