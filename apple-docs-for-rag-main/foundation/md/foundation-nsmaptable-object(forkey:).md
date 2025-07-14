

- Foundation
- NSMapTable
-  object(forKey:) 

Instance Method

# object(forKey:)

Returns a the value associated with a given key.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func object(forKey aKey: KeyType?) -> ObjectType?
```

## Parameters 

`aKey`  

The key for which to return the corresponding value.

## Return Value

The value associated with `aKey`, or `nil` if no value is associated with `aKey`.

## See Also

### Accessing Content

func keyEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each key in the map table.

func objectEnumerator() -> NSEnumerator?

Returns an enumerator object that lets you access each value in the map table.

var count: Int

The number of key-value pairs in the map table.

