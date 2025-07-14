

- AppKit
-  NSCollectionLayoutSectionOrthogonalScrollingBehavior 

Enumeration

# NSCollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

macOS 10.15+

``` source
enum NSCollectionLayoutSectionOrthogonalScrollingBehavior
```

## Overview

By default, each section lays out its content along the main axis of its layout, defined by the layout configuration’s scrollDirection property. You can change this behavior for a particular section by setting its orthogonalScrollingBehavior property to a different value than its default NSCollectionLayoutSectionOrthogonalScrollingBehavior.none. Setting any other value for this property makes the section lay out its content orthogonally to the main layout axis.

## Topics

### Enumeration Cases

case none

The section does not allow users to scroll its content orthogonally.

case continuous

The section allows users to scroll its content orthogonally with continuous scrolling.

case continuousGroupLeadingBoundary

The section allows users to scroll its content orthogonally, coming to a natural stop at the leading boundary of the visible group.

case paging

The section allows users to page its content orthogonally.

case groupPaging

The section allows users to page its content orthogonally one group at a time.

case groupPagingCentered

The section allows users to page its content orthogonally one group at a time, centering each group.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
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

class NSCollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

typealias NSCollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

