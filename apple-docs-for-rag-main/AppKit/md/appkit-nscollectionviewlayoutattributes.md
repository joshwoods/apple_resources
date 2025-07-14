

- AppKit
-  NSCollectionViewLayoutAttributes 

Class

# NSCollectionViewLayoutAttributes

An object that contains layout-related attributes for an element in a collection view.

macOS 10.11+

``` source
@MainActor
class NSCollectionViewLayoutAttributes
```

## Overview

During the layout, the layout object creates instances of NSCollectionViewLayoutAttributes for each element displayed in the collection view. The layout attributes describe the position of an element and other information such as its alpha and position on the z axis. The collection view later applies the layout attributes to the onscreen elements.

The only time you interact with layout attribute objects is when you implement a custom layout, and the interactions are straightforward. When asked for layout attributes for a specific element, your layout object uses the methods of this class to create an appropriate instance of the class based on the type of the requested element. It then configures the properties of the object and returns it to the requester.

### Subclassing Notes

If you implement a custom layout object and your layout object requires additional attributes, you can subclass `NSCollectionViewLayoutAttributes` and add custom properties to your subclass. In your subclass, be sure to do the following:

- Provide an init() method with no parameters to initialize your subclass.

- Implement support for the NSCopying protocol. The collection view caches layout attribute objects for later use.

- Override the inherited isEqual(_:) method to perform any relevant equality checks.

Supporting equality checks is important because of how the collection view manages layout attributes. As an optimization, the collection view applies layout attributes only when they change. When the layout object returns a layout attributes object, the collection view checks to see if the new attributes are equal to any cached attributes. Therefore, if you want to include any new properties in the equality check, you must override the isEqual(_:) method.

In addition to defining your `NSCollectionViewLayoutAttributes` subclass, override the layoutAttributesClass method of your layout object. That method is a funnel point for creating new layout attribute objects. Returning your custom class from that method ensures that the correct class is instantiated.

## Topics

### Creating Layout Attributes

convenience init(forItemWith: IndexPath)

Creates and returns a layout attributes object for the item at the specified index path.

convenience init(forSupplementaryViewOfKind: NSCollectionView.SupplementaryElementKind, with: IndexPath)

Creates and returns a layout attributes object for a supplementary view based on the specified information.

convenience init(forDecorationViewOfKind: NSCollectionView.DecorationElementKind, with: IndexPath)

Creates and returns a layout attributes object for a decoration view based on the specified information.

convenience init(forInterItemGapBefore: IndexPath)

Creates and returns a layout attributes object for an inter-item gap view at the specified index path.

typealias DecorationElementKind

### Identifying the Element

var representedElementCategory: NSCollectionElementCategory

The type of the element.

var indexPath: IndexPath?

The index path of the element.

var representedElementKind: String?

The identifier for specific elements of your collection view interface.

class let elementKindInterItemGapIndicator: String

The element kind string assigned to the attributes object when it represents an inter-item gap.

class let elementKindSectionFooter: String

A supplementary view that acts as a footer for a given section.

class let elementKindSectionHeader: String

A supplementary view that acts as a header for a given section.

### Accessing the Layout Attributes

var frame: NSRect

The frame rectangle of the element.

var size: NSSize

The size of the element.

var alpha: CGFloat

The transparency of the element.

var isHidden: Bool

A Boolean value indicating whether the element is hidden.

var zIndex: Int

The element’s position on the z axis.

### Constants

enum NSCollectionElementCategory

Constants specifying the type of element in the collection view.

Inter-Item Gap Support

Constant for supporting inter-item gaps.

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

class NSCollectionViewLayout

An abstract base class that you subclass and use to generate layout information for a collection view.

class NSCollectionViewCompositionalLayout

A layout object that lets you combine items in highly adaptive and flexible visual arrangements.

class NSCollectionViewCompositionalLayoutConfiguration

An object that defines scroll direction, section spacing, and headers or footers for the layout.

typealias NSCollectionViewCompositionalLayoutSectionProvider

A closure that creates and returns each of the layout’s sections.

enum NSCollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

