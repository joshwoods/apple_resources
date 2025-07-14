

- Foundation
- NSArray
-  setValue(\_:forKey:) 

Instance Method

# setValue(\_:forKey:)

Invokes setValue(_:forKey:) on each of the array’s items using the specified `value` and `key`.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

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

### Key-Value Coding

func value(forKey: String) -> Any

Returns an array containing the results of invoking value(forKey:) using `key` on each of the array’s objects.

