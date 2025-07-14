

- AppKit
-  NSCollectionViewCompositionalLayoutConfiguration 

Class

# NSCollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

macOS 10.15+

``` source
@MainActor
class NSCollectionViewCompositionalLayoutConfiguration
```

## Overview

You use a layout configuration to modify a collection view layout’s default scroll direction, add extra spacing between each section of the layout, and add headers or footers to the entire layout.

You can pass in this configuration when creating an NSCollectionViewCompositionalLayout, or you can set the configuration property on an existing layout. If you modify the configuration on an existing layout, the system invalidates the layout so that it will be updated with the new configuration.

```
let headerFooterSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(1.0),
                                             heightDimension: .estimated(44))

let header = NSCollectionLayoutBoundarySupplementaryItem(layoutSize: headerFooterSize,
                                                        elementKind: "header",
                                                          alignment: .top)
let footer = NSCollectionLayoutBoundarySupplementaryItem(layoutSize: headerFooterSize,
                                                        elementKind: "footer",
                                                          alignment: .bottom)

let config = NSCollectionViewCompositionalLayoutConfiguration()
config.interSectionSpacing = 20
config.scrollDirection = .horizontal
config.boundarySupplementaryItems = [header, footer]
```

## Topics

### Specifying Scroll Direction

var scrollDirection: NSCollectionView.ScrollDirection

The axis that the content in the collection view layout scrolls along.

### Configuring Spacing

var interSectionSpacing: CGFloat

The amount of space between the sections in the layout.

### Configuring Additional Views

var boundarySupplementaryItems: [NSCollectionLayoutBoundarySupplementaryItem]

An array of the supplementary items that are associated with the boundary edges of the entire layout, such as global headers and footers.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Layouts

Implementing modern collection views

Bring compositional layouts to your app and simplify updating your user interface with diffable data sources.

class NSCollectionViewFlowLayout

A layout that organizes items into a flexible and configurable arrangement.

protocol NSCollectionViewDelegateFlowLayout

A set of methods that a delegate implements to provide layout information to a flow layout object in a collection view.

class NSCollectionViewGridLayout

A layout that displays a single section of items in a row and column grid.

class NSCollectionViewTransitionLayout

An object that implements custom behaviors when changing from one layout to another in a collection view.

class NSCollectionViewLayoutAttributes

An object that contains layout-related attributes for an element in a collection view.

class NSCollectionViewLayout

An abstract base class that you subclass and use to generate layout information for a collection view.

class NSCollectionViewCompositionalLayout

A layout object that lets you combine items in highly adaptive and flexible visual arrangements.

typealias NSCollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

enum NSCollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

