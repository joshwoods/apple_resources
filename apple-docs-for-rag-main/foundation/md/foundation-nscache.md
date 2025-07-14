

- Foundation
-  NSCache 

Class

# NSCache

A mutable collection you use to temporarily store transient key-value pairs that are subject to eviction when resources are low.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSCache where KeyType : AnyObject, ObjectType : AnyObject
```

## Overview

Cache objects differ from other mutable collections in a few ways:

- The NSCache class incorporates various auto-eviction policies, which ensure that a cache doesn’t use too much of the system’s memory. If memory is needed by other applications, these policies remove some items from the cache, minimizing its memory footprint.

- You can add, remove, and query items in the cache from different threads without having to lock the cache yourself.

- Unlike an NSMutableDictionary object, a cache does not copy the key objects that are put into it.

You typically use NSCache objects to temporarily store objects with transient data that are expensive to create. Reusing these objects can provide performance benefits, because their values do not have to be recalculated. However, the objects are not critical to the application and can be discarded if memory is tight. If discarded, their values will have to be recomputed again when needed.

Objects that have subcomponents that can be discarded when not being used can adopt the NSDiscardableContent protocol to improve cache eviction behavior. By default, NSDiscardableContent objects in a cache are automatically removed if their content is discarded, although this automatic removal policy can be changed. If an NSDiscardableContent object is put into the cache, the cache calls discardContentIfPossible() on it upon its removal.

## Topics

### Managing the Name

var name: String

The name of the cache.

### Managing Cache Size

var countLimit: Int

The maximum number of objects the cache should hold.

var totalCostLimit: Int

The maximum total cost that the cache can hold before it starts evicting objects.

### Managing Discardable Content

var evictsObjectsWithDiscardedContent: Bool

Whether the cache will automatically evict discardable-content objects whose content has been discarded.

protocol NSDiscardableContent

You implement this protocol when a class’s objects have subcomponents that can be discarded when not being used, thereby giving an application a smaller memory footprint.

### Managing the Delegate

var delegate: (any NSCacheDelegate)?

The cache’s delegate.

protocol NSCacheDelegate

The delegate of an NSCache object implements this protocol to perform specialized actions when an object is about to be evicted or removed from the cache.

### Getting a Cached Value

func object(forKey: KeyType) -> ObjectType?

Returns the value associated with a given key.

### Adding and Removing Cached Values

func setObject(ObjectType, forKey: KeyType)

Sets the value of the specified key in the cache.

func setObject(ObjectType, forKey: KeyType, cost: Int)

Sets the value of the specified key in the cache, and associates the key-value pair with the specified cost.

func removeObject(forKey: KeyType)

Removes the value of the specified key in the cache.

func removeAllObjects()

Empties the cache.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Purgeable Collections

class NSPurgeableData

A mutable data object containing bytes that can be discarded when they’re no longer needed.

