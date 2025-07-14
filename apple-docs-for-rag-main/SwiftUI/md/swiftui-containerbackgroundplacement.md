

- SwiftUI
-  ContainerBackgroundPlacement 

Structure

# ContainerBackgroundPlacement

The placement of a container background.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ContainerBackgroundPlacement
```

## Overview

This method controls where to place a background that you specify with the containerBackground(_:for:) or containerBackground(for:alignment:content:) modifier.

## Topics

### Getting placements

static let navigation: ContainerBackgroundPlacement

A background placement inside a NavigationStack or NavigationSplitView.

static let tabView: ContainerBackgroundPlacement

A background placement inside a TabView.

static let widget: ContainerBackgroundPlacement

The container background placement for a widget.

### Getting StoreKit placements

static var subscriptionStore: ContainerBackgroundPlacement

An automatic placement within a subscription store view, based on the view’s context.

static var subscriptionStoreFullHeight: ContainerBackgroundPlacement

A background placement that spans the full height of a subscription store view.

static var subscriptionStoreHeader: ContainerBackgroundPlacement

A background placement behind the marketing content of a subscription store view.

### Type Properties

static let navigationSplitView: ContainerBackgroundPlacement

A background placement behind the content of a NavigationSplitView.

static let window: ContainerBackgroundPlacement

A background placement inside a Window or WindowGroup

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Layering views

Adding a background to your view

Compose a background behind your view and extend it beyond the safe area insets.

struct ZStack

A view that overlays its subviews, aligning them in both axes.

func zIndex(Double) -> some View

Controls the display order of overlapping views.

func background&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify behind this view.

func background&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to a style.

func background(ignoresSafeAreaEdges: Edge.Set) -> some View

Sets the view’s background to the default background style.

func background(_:in:fillStyle:)

Sets the view’s background to an insettable shape filled with a style.

func background(in:fillStyle:)

Sets the view’s background to an insettable shape filled with the default background style.

func overlay&lt;V>(alignment: Alignment, content: () -> V) -> some View

Layers the views that you specify in front of this view.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

var backgroundMaterial: Material?

The material underneath the current view.

func containerBackground&lt;S>(S, for: ContainerBackgroundPlacement) -> some View

Sets the container background of the enclosing container using a view.

func containerBackground&lt;V>(for: ContainerBackgroundPlacement, alignment: Alignment, content: () -> V) -> some View

Sets the container background of the enclosing container using a view.

