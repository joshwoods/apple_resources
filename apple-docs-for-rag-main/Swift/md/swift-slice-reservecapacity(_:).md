

- Swift
- Slice
-  reserveCapacity(\_:) 

Instance Method

# reserveCapacity(\_:)

Prepares the collection to store the specified number of elements, when doing so is appropriate for the underlying type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func reserveCapacity(_ n: Int)
```

## Parameters 

`n`  

The requested number of elements to store.

## Discussion

If you will be adding a known number of elements to a collection, use this method to avoid multiple reallocations. A type that conforms to `RangeReplaceableCollection` can choose how to respond when this method is called. Depending on the type, it may make sense to allocate more or less storage than requested or to take no action at all.

