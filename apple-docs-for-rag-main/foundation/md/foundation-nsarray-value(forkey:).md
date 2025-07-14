

- Foundation
- NSArray
-  value(forKey:) 

Instance Method

# value(forKey:)

Returns an array containing the results of invoking value(forKey:) using `key` on each of the array’s objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func value(forKey key: String) -> Any
```

## Parameters 

`key`  

The key to retrieve.

## Return Value

The value of the retrieved key.

## Discussion

The returned array contains `NSNull` elements for each object that returns `nil`.

## See Also

### Key-Value Coding

func setValue(Any?, forKey: String)

Invokes setValue(_:forKey:) on each of the array’s items using the specified `value` and `key`.

