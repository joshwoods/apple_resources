

- Swift
- RangeReplaceableCollection
-  removeAll(keepingCapacity:) 

Instance Method

# removeAll(keepingCapacity:)

Removes all elements from the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeAll(keepingCapacity keepCapacity: Bool)
```

**Required** Default implementation provided.

## Parameters 

`keepCapacity`  

Pass `true` to request that the collection avoid releasing its storage. Retaining the collection’s storage can be a useful optimization when you’re planning to grow the collection again. The default value is `false`.

## Discussion

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

## Default Implementations

### RangeReplaceableCollection Implementations

func removeAll(keepingCapacity: Bool)

Removes all elements from the collection.

