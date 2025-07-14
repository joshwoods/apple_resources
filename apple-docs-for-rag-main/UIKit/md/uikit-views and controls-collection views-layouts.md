

- UIKit
- Views and controls
- Collection views
-  Layouts 

API Collection

# Layouts

Arrange your collection view content in a highly configurable layout.

## Overview

A collection view *layout* defines the visual arrangement of the content in your collection. Layouts are designed to be flexible to let you create any kind of arrangement you need for your content, from simple to complex. The simplest type of collection view layout displays its items in a grid, but you can define layouts to arrange items however you like. For example, you might create a layout where items are arranged in a circle or vary in size. You can also change layouts dynamically at runtime whenever you need to present items differently, such as when a user rotates the device.

Collection view layouts are customizable and highly visual. For example, the App Store app uses a single collection view with custom layouts per section to showcase different kinds of content.

For design guidance, see Human Interface Guidelines.

## Topics

### Essentials

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

class UICollectionViewCompositionalLayout

A layout object that lets you combine items in highly adaptive and flexible visual arrangements.

### Components

class NSCollectionLayoutItem

The most basic component of a collection view’s layout.

class NSCollectionLayoutGroup

A container for a set of items that lays out the items along a path.

class NSCollectionLayoutSection

A container that combines a set of groups into distinct visual groupings.

### Size and spacing

class NSCollectionLayoutDimension

An individual dimension representing an item’s width or height in a collection view.

class NSCollectionLayoutSize

The width and the height of an item in a collection view.

class NSCollectionLayoutSpacing

An object that defines the space between or around items in a collection view.

class NSCollectionLayoutEdgeSpacing

An object that defines the space around the edges of items in a collection view.

protocol NSCollectionLayoutContainer

A protocol used to provide information about the size and content insets of a layout’s container.

### Configuration

class UICollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

typealias UICollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

protocol NSCollectionLayoutEnvironment

A protocol used to provide information about the layout’s container and environment traits, such as size classes and display scale factor.

### Interaction

enum UICollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

### Appearance

class NSCollectionLayoutAnchor

An object that defines how to attach a supplementary item to an item in a collection view.

class NSCollectionLayoutSupplementaryItem

An object used to add an extra visual decoration to an item in a collection view.

class NSCollectionLayoutBoundarySupplementaryItem

An object used to add headers or footers to a collection view.

class NSCollectionLayoutDecorationItem

An object used to add a background to a section of a collection view.

### Advanced layouts

class NSCollectionLayoutGroupCustomItem

An item used in a group with a custom layout arrangement.

typealias NSCollectionLayoutGroupCustomItemProvider

A closure that creates and returns each of the custom group’s items.

### Layout updates

protocol NSCollectionLayoutVisibleItem

An item that’s currently visible within the bounds of a section.

typealias NSCollectionLayoutSectionVisibleItemsInvalidationHandler

A closure called before each layout cycle to allow modification of items in a section immediately before they’re displayed.

class UICollectionViewUpdateItem

An object that describes a single change to make to an item in a collection view.

class UICollectionViewFocusUpdateContext

A context object that stores information specific to a focus update in a collection view.

class UICollectionViewLayoutInvalidationContext

A context object that declares which parts of your layout need to be updated when the layout is invalidated.

### Manual layouts

Customizing collection view layouts

Customize a view layout by changing the size of cells in the flow or implementing a mosaic style.

class UICollectionViewLayout

An abstract base class for generating layout information for a collection view.

class UICollectionViewFlowLayout

A layout object that organizes items into a grid with optional header and footer views for each section.

class UICollectionViewTransitionLayout

A special type of layout object that lets you implement behaviors when changing from one layout to another in your collection view.

class UICollectionViewLayoutAttributes

A layout object that manages the layout-related attributes for a given item in a collection view.

class UICollectionViewFlowLayoutInvalidationContext

A set of properties for determining whether to recompute the size of items or their position in the layout.

### Data

struct NSDiffableDataSourceSnapshot

A representation of the state of the data in a view at a specific point in time.

## See Also

### Layouts

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

