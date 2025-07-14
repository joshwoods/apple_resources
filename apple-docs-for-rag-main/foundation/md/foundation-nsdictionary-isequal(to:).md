

- Foundation
- NSDictionary
-  isEqual(to:) 

Instance Method

# isEqual(to:)

Returns a Boolean value that indicates whether the contents of the receiving dictionary are equal to the contents of another given dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func isEqual(to otherDictionary: [AnyHashable : Any]) -> Bool
```

## Parameters 

`otherDictionary`  

The dictionary with which to compare the receiving dictionary.

## Return Value

true if the contents of `otherDictionary` are equal to the contents of the receiving dictionary, otherwise false.

## Discussion

Two dictionaries have equal contents if they each hold the same number of entries and, for a given key, the corresponding value objects in each dictionary satisfy the isEqual(_:) test.

## See Also

### Related Documentation

func isEqual(_ object: Any?) -> Bool

Returns a Boolean value that indicates whether the receiver and a given object are equal.

