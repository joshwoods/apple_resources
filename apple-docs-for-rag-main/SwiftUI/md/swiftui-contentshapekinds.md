

- SwiftUI
-  ContentShapeKinds 

Structure

# ContentShapeKinds

A kind for the content shape of a view.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ContentShapeKinds
```

## Overview

The kind is used by the system to influence various effects, hit-testing, and more.

## Topics

### Getting shape kinds

static let interaction: ContentShapeKinds

The kind for hit-testing and accessibility.

static let dragPreview: ContentShapeKinds

The kind for drag and drop previews.

static let contextMenuPreview: ContentShapeKinds

The kind for context menu previews.

static let focusEffect: ContentShapeKinds

The kind for the focus effect.

static let hoverEffect: ContentShapeKinds

The kind for hover effects.

static let accessibility: ContentShapeKinds

The kind for accessibility visuals and sorting.

### Creating a set of options

init(rawValue: Int)

Creates a content shape kind.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Controlling hit testing

func allowsTightening(Bool) -> some View

Sets whether text in this view can compress the space between characters when necessary to fit text in a line.

func contentShape&lt;S>(S, eoFill: Bool) -> some View

Defines the content shape for hit testing.

func contentShape&lt;S>(ContentShapeKinds, S, eoFill: Bool) -> some View

Sets the content shape for this view.

