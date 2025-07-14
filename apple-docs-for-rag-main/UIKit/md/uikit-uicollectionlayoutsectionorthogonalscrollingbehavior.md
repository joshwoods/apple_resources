

- UIKit
-  UICollectionLayoutSectionOrthogonalScrollingBehavior 

Enumeration

# UICollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
enum UICollectionLayoutSectionOrthogonalScrollingBehavior
```

## Overview

By default, each section lays out its content along the main axis of its layout, defined by the layout configuration’s scrollDirection property. You can change this behavior for a particular section by setting its orthogonalScrollingBehavior property to a different value than its default UICollectionLayoutSectionOrthogonalScrollingBehavior.none. Setting any other value for this property makes the section lay out its content orthogonally to the main layout axis.

## Topics

### Constants

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

