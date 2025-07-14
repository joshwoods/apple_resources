

- AppKit
-  NSCollectionLayoutSection 

Class

# NSCollectionLayoutSection

A container that combines a set of groups into distinct visual groupings.

macOS 10.15+

``` source
@MainActor
class NSCollectionLayoutSection
```

## Overview

A collection view layout has one or more sections. Sections provide a way to separate the layout into distinct pieces.

Each section can have the same layout or a different layout than the other sections in the collection view. A section’s layout is determined by the properties of the group (NSCollectionLayoutGroup) that’s used to create the section.

In the Photos app, each section in the Years page uses the same layout. In the App Store, the Apps page displays several sections with different content arrangements.

Each section can have its own background, header, and footer to distinguish it from other sections.

## Topics

### Creating a section

convenience init(group: NSCollectionLayoutGroup)

Creates a section containing the specified group.

### Specifying scrolling behavior

var orthogonalScrollingBehavior: NSCollectionLayoutSectionOrthogonalScrollingBehavior

The section’s scrolling behavior in relation to the main layout axis.

### Configuring section spacing

var interGroupSpacing: CGFloat

The amount of space between the groups in the section.

var contentInsets: NSDirectionalEdgeInsets

The amount of space between the content of the section and its boundaries.

### Configuring additional views

var boundarySupplementaryItems: [NSCollectionLayoutBoundarySupplementaryItem]

An array of the supplementary items that are associated with the boundary edges of the section, such as headers and footers.

var decorationItems: [NSCollectionLayoutDecorationItem]

An array of the decoration items that are anchored to the section, such as background decoration views.

### Rendering items

var visibleItemsInvalidationHandler: NSCollectionLayoutSectionVisibleItemsInvalidationHandler?

A closure called before each layout cycle to allow modification of the items in the section immediately before they’re displayed.

### Deprecated

var supplementariesFollowContentInsets: Bool

A Boolean value that indicates whether the section’s supplementary items follow the specified content insets for the section.

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

### Components

class NSCollectionLayoutItem

The most basic component of a collection view’s layout.

class NSCollectionLayoutGroup

A container for a set of items that lays out the items along a path.

