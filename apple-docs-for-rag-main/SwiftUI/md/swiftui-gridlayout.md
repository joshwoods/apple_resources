

- SwiftUI
-  GridLayout 

Structure

# GridLayout

A grid that you can use in conditional layouts.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@frozen
struct GridLayout
```

## Overview

This layout container behaves like a Grid, but conforms to the Layout protocol so you can use it in the conditional layouts that you construct with AnyLayout. If you don’t need a conditional layout, use Grid instead.

## Topics

### Creating a grid

init(alignment: Alignment, horizontalSpacing: CGFloat?, verticalSpacing: CGFloat?)

Creates a grid with the specified spacing and alignment.

### Getting the grid’s properties

var alignment: Alignment

The alignment of subviews.

var horizontalSpacing: CGFloat?

The horizontal distance between adjacent subviews.

var verticalSpacing: CGFloat?

The vertical distance between adjacent subviews.

### Type Aliases

typealias Body

### Default Implementations

Layout Implementations

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

struct ZStackLayout

An overlaying container that you can use in conditional layouts.

