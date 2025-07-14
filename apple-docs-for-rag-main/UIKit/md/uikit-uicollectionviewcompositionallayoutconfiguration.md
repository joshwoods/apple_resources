

- UIKit
-  UICollectionViewCompositionalLayoutConfiguration 

Class

# UICollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UICollectionViewCompositionalLayoutConfiguration
```

## Overview

You use a layout configuration to modify a collection view layout’s default scroll direction, add extra spacing between each section of the layout, and add headers or footers to the entire layout.

You can pass in this configuration when creating a UICollectionViewCompositionalLayout, or you can set the configuration property on an existing layout. If you modify the configuration on an existing layout, the system invalidates the layout so that it will be updated with the new configuration.

- Swift
- Objective-C

```
let headerFooterSize = NSCollectionLayoutSize(widthDimension: .fractionalWidth(1.0),
                                             heightDimension: .estimated(44))

let header = NSCollectionLayoutBoundarySupplementaryItem(layoutSize: headerFooterSize,
                                                        elementKind: "header",
                                                          alignment: .top)
let footer = NSCollectionLayoutBoundarySupplementaryItem(layoutSize: headerFooterSize,
                                                        elementKind: "footer",
                                                          alignment: .bottom)

let config = UICollectionViewCompositionalLayoutConfiguration()
config.interSectionSpacing = 20
config.scrollDirection = .horizontal
config.boundarySupplementaryItems = [header, footer]
```

```
NSCollectionLayoutSize *headerFooterSize = [NSCollectionLayoutSize sizeWithWidthDimension:[NSCollectionLayoutDimension fractionalWidthDimension:1.0] heightDimension:[NSCollectionLayoutDimension estimatedDimension:44.0]];

NSCollectionLayoutBoundarySupplementaryItem *header = [NSCollectionLayoutBoundarySupplementaryItem boundarySupplementaryItemWithLayoutSize:headerFooterSize elementKind:@"header" alignment:NSRectAlignmentTop];

NSCollectionLayoutBoundarySupplementaryItem *footer = [NSCollectionLayoutBoundarySupplementaryItem boundarySupplementaryItemWithLayoutSize:headerFooterSize elementKind:@"footer" alignment:NSRectAlignmentBottom];

UICollectionViewCompositionalLayoutConfiguration *config = [[UICollectionViewCompositionalLayoutConfiguration alloc] init];
[config setInterSectionSpacing:20.0];
[config setScrollDirection:UICollectionViewScrollDirectionHorizontal];
[config setBoundarySupplementaryItems:@[header, footer]];
```

## Topics

### Specifying scroll direction

var scrollDirection: UICollectionView.ScrollDirection

The axis that the content in the collection view layout scrolls along.

### Configuring spacing

var interSectionSpacing: CGFloat

The amount of space between the sections in the layout.

var contentInsetsReference: UIContentInsetsReference

The boundary to reference when defining content insets.

enum UIContentInsetsReference

Constants that describe the reference point of the content insets.

### Configuring additional views

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

### Configuration

typealias UICollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

protocol NSCollectionLayoutEnvironment

A protocol used to provide information about the layout’s container and environment traits, such as size classes and display scale factor.

