

- Foundation
- NSOrderedSet
-  setValue(\_:forKey:) 

Instance Method

# setValue(\_:forKey:)

Invokes `setValue:forKey:` on each of the receiver’s members using the specified value and key

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setValue(
    _ value: Any?,
    forKey key: String
)
```

## Parameters 

`value`  

The object value.

`key`  

The key to store the value.

## See Also

### Key-Value Coding Support

func value(forKey: String) -> Any

Returns an ordered set containing the results of invoking `valueForKey:` using key on each of the ordered set’s objects.

