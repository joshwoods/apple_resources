

- UIKit
-  NSCollectionLayoutSection 

Class

# NSCollectionLayoutSection

A container that combines a set of groups into distinct visual groupings.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

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

static func list(using: UICollectionLayoutListConfiguration, layoutEnvironment: any NSCollectionLayoutEnvironment) -> NSCollectionLayoutSection

Creates a list section with the specified list configuration and layout environment.

class func orthogonalLayoutSectionForMediaItems() -> NSCollectionLayoutSection

Creates an orthogonally scrolling section with system default spacing.

### Specifying scrolling behavior

var orthogonalScrollingBehavior: UICollectionLayoutSectionOrthogonalScrollingBehavior

The section’s scrolling behavior in relation to the main layout axis.

var orthogonalScrollingProperties: UICollectionLayoutSectionOrthogonalScrollingProperties

The section’s orthogonal scrolling properties.

class UICollectionLayoutSectionOrthogonalScrollingProperties

An object that specifies properties for a layout section that scrolls orthogonally in relation to the main layout axis.

### Configuring section spacing

var interGroupSpacing: CGFloat

The amount of space between the groups in the section.

var contentInsets: NSDirectionalEdgeInsets

The amount of space between the content of the section and its boundaries.

var contentInsetsReference: UIContentInsetsReference

The boundary to reference when defining content insets.

var supplementaryContentInsetsReference: UIContentInsetsReference

The reference boundary for content insets on boundary supplementary items.

enum UIContentInsetsReference

Constants that describe the reference point of the content insets.

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

Deprecated

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

