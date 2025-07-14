

- Objective-C Runtime
- NSObject
-  removeValue(at:fromPropertyWithKey:) 

Instance Method

# removeValue(at:fromPropertyWithKey:)

Removes the object at the specified index from the collection specified by the passed key.

Mac CatalystmacOS

``` source
func removeValue(
    at index: Int,
    fromPropertyWithKey key: String
)
```

## Discussion

The method `removeFromAtIndex:` is invoked if it exists. If no corresponding scripting-KVC-compliant method (`-removeFromAtIndex:`) is found, this method invokes `-mutableArrayValueForKey:` and mutates the result.

Note

Prior to OS X version 10.4, this method did not invoke `-mutableArrayValueForKey:`.

## See Also

### Indexed access

func insertValue(Any, at: Int, inPropertyWithKey: String)

Inserts an object at the specified index in the collection specified by the passed key.

func replaceValue(at: Int, inPropertyWithKey: String, withValue: Any)

Replaces the object at the specified index in the collection specified by the passed key.

func value(at: Int, inPropertyWithKey: String) -> Any?

Retrieves an indexed object from the collection specified by the passed key.

