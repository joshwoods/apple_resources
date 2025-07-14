

- AppKit
-  NSCollectionViewTransitionLayout 

Class

# NSCollectionViewTransitionLayout

An object that implements custom behaviors when changing from one layout to another in a collection view.

macOS 10.11+

``` source
@MainActor
class NSCollectionViewTransitionLayout
```

## Overview

Transition layout objects are commonly used to implement interactive transitions between layouts, where the transition itself is driven by a gesture recognizer.

Note

In macOS 10.11, collection views do not provide built-in support for driving layout transitions.

## Topics

### Initializing the Transition Layout Object

init(currentLayout: NSCollectionViewLayout, nextLayout: NSCollectionViewLayout)

Initializes and returns the transition layout object.

### Updating the Transition Information

var transitionProgress: CGFloat

The completion percentage of the transition.

func updateValue(CGFloat, forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey)

Sets the value of a key whose value you use during the animation.

func value(forAnimatedKey: NSCollectionViewTransitionLayout.AnimatedKey) -> CGFloat

Returns the most recently set value for the specified key.

typealias AnimatedKey

### Accessing the Layout Objects

var currentLayout: NSCollectionViewLayout

The collection view’s current layout object.

var nextLayout: NSCollectionViewLayout

The collection view’s new layout object.

## Relationships

### Inherits From

- NSCollectionViewLayout

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
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

enum NSCollectionLayoutSectionOrthogonalScrollingBehavior

The scrolling behavior of the layout’s sections in relation to the main layout axis.

