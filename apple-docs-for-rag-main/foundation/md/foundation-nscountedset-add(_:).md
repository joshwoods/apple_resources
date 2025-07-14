

- Foundation
- NSCountedSet
-  add(\_:) 

Instance Method

# add(\_:)

Adds a given object to the set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func add(_ object: Any)
```

## Parameters 

`object`  

The object to add to the set.

## Discussion

If `object` is already a member, add(_:) increments the count associated with the object. If `object` is not already a member, it is sent a retain message.

## See Also

### Adding and Removing Entries

func remove(Any)

Removes a given object from the set.

