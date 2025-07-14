

- Objective-C Runtime
- NSObject
-  insertValue(\_:at:inPropertyWithKey:) 

Instance Method

# insertValue(\_:at:inPropertyWithKey:)

Inserts an object at the specified index in the collection specified by the passed key.

Mac CatalystmacOS

``` source
func insertValue(
    _ value: Any,
    at index: Int,
    inPropertyWithKey key: String
)
```

## Discussion

The method `insertIn:atIndex:` is invoked if it exists. If no corresponding scripting-KVC-compliant method (`insertIn:atIndex:` ) is found, this method invokes `mutableArrayValueForKey:` and mutates the result.

Note

Prior to OS X version 10.4, this method did not invoke `-mutableArrayValueForKey:`.

## See Also

### Indexed access

func removeValue(at: Int, fromPropertyWithKey: String)

Removes the object at the specified index from the collection specified by the passed key.

func replaceValue(at: Int, inPropertyWithKey: String, withValue: Any)

Replaces the object at the specified index in the collection specified by the passed key.

func value(at: Int, inPropertyWithKey: String) -> Any?

Retrieves an indexed object from the collection specified by the passed key.

