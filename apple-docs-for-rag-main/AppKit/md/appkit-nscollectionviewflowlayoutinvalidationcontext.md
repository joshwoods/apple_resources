

- AppKit
-  NSCollectionViewFlowLayoutInvalidationContext 

Class

# NSCollectionViewFlowLayoutInvalidationContext

An object that identifies the portions of a flow layout object that need to be updated.

macOS 10.11+

``` source
@MainActor
class NSCollectionViewFlowLayoutInvalidationContext
```

## Overview

Layout objects use invalidation contexts to optimize the layout process and avoid unnecessary work. You use this class to specify whether the NSCollectionViewFlowLayout object should fetch new size information from its delegate. You can also prevent the flow layout object from updating its layout information altogether.

When you want to invalidate your flow layout object, call the invalidationContextClass method of your layout object and instantiate the resulting class. (The implementation of that method in NSCollectionViewFlowLayout returns this class.) After instantiating this class, set the properties to appropriate values and pass the object to the invalidateLayout(with:) method of the layout object.

## Topics

### Invalidating the Flow Layout

var invalidateFlowLayoutAttributes: Bool

A Boolean value indicating whether the flow layout object should invalidate its current attributes.

var invalidateFlowLayoutDelegateMetrics: Bool

A Boolean value indicating whether the flow layout object should fetch new size information from its delegate.

## Relationships

### Inherits From

- NSCollectionViewLayoutInvalidationContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Updates

class NSCollectionViewUpdateItem

A description of a single change to make to an item in a collection view.

class NSCollectionViewLayoutInvalidationContext

An object that identifies the portions of your layout that need to be updated.

