

- Combine
- Cancellable
-  store(in:) 

Instance Method

# store(in:)

Stores this cancellable instance in the specified collection.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func store(in collection: inout C) where C : RangeReplaceableCollection, C.Element == AnyCancellable
```

## Parameters 

`collection`  

The collection in which to store this Cancellable.

## See Also

### Storing Cancellable Instances

func store(in: inout Set&lt;AnyCancellable>)

Stores this cancellable instance in the specified set.

