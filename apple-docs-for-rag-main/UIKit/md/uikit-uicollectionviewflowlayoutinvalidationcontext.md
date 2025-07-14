

- UIKit
-  UICollectionViewFlowLayoutInvalidationContext 

Class

# UICollectionViewFlowLayoutInvalidationContext

A set of properties for determining whether to recompute the size of items or their position in the layout.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
class UICollectionViewFlowLayoutInvalidationContext
```

## Overview

The flow layout object creates instances of this class when it needs to invalidate its contents in response to changes. You can also create instances when invalidating the flow layout manually.

## Topics

### Specifying what to invalidate

var invalidateFlowLayoutDelegateMetrics: Bool

A Boolean indicating whether to recompute the size of items and views in the layout.

var invalidateFlowLayoutAttributes: Bool

A Boolean indicating whether to recompute the layout attributes for items and views in the layout.

## Relationships

### Inherits From

- UICollectionViewLayoutInvalidationContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

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

