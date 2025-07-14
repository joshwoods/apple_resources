

- Foundation
- NSOrderedSet
-  value(forKey:) 

Instance Method

# value(forKey:)

Returns an ordered set containing the results of invoking `valueForKey:` using key on each of the ordered set’s objects.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forKey key: String) -> Any
```

## Parameters 

`key`  

The key to retrieve.

## Return Value

The ordered set of the values for the retrieved key. The returned ordered set might not have the same number of members as the receiver.

## Discussion

The returned ordered set will not contain any elements corresponding to instances of `valueForKey:` returning `nil`, nor will it contain duplicates.

## See Also

### Key-Value Coding Support

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the receiver’s members using the specified value and key

