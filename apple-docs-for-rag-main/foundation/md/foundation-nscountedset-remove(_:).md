

- Foundation
- NSCountedSet
-  remove(\_:) 

Instance Method

# remove(\_:)

Removes a given object from the set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func remove(_ object: Any)
```

## Parameters 

`object`  

The object to remove from the set.

## Discussion

If `object` is present in the set, decrements the count associated with it. If the count is decremented to `0`, `object` is removed from the set. remove(_:) does nothing if `object` is not present in the set.

## See Also

### Related Documentation

func count(for: Any) -> Int

Returns the count associated with a given object in the set.

### Adding and Removing Entries

func add(Any)

Adds a given object to the set.

