

- Objective-C Runtime
- NSObject
-  replaceValue(at:inPropertyWithKey:withValue:) 

Instance Method

# replaceValue(at:inPropertyWithKey:withValue:)

Replaces the object at the specified index in the collection specified by the passed key.

Mac CatalystmacOS

``` source
func replaceValue(
    at index: Int,
    inPropertyWithKey key: String,
    withValue value: Any
)
```

## Discussion

The method `replaceIn:atIndex:` is invoked if it exists. If no corresponding scripting-KVC-compliant method (`-replaceInatIndex:`) is found, this method invokes `-mutableArrayValueForKey:` and mutates the result.

Note

Prior to OS X version 10.4, this method did not invoke `-mutableArrayValueForKey:`.

## See Also

### Indexed access

func insertValue(Any, at: Int, inPropertyWithKey: String)

Inserts an object at the specified index in the collection specified by the passed key.

func removeValue(at: Int, fromPropertyWithKey: String)

Removes the object at the specified index from the collection specified by the passed key.

func value(at: Int, inPropertyWithKey: String) -> Any?

Retrieves an indexed object from the collection specified by the passed key.

