

- Foundation
- NSMapTable
-  objectEnumerator() 

Instance Method

# objectEnumerator()

Returns an enumerator object that lets you access each value in the map table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objectEnumerator() -> NSEnumerator?
```

## Return Value

An enumerator object that lets you access each value in the map table.

## Discussion

The following code fragment illustrates how you might use the method.

```
NSEnumerator *enumerator = [myMapTable objectEnumerator];
id value;

while ((value = [enumerator nextObject])) {
    /* code that acts on the map table's values */
}
```

### Special Considerations

It is more efficient to use the fast enumeration protocol (see NSFastEnumeration).

## See Also

### Accessing Content

func object(forKey: KeyType?) -> ObjectType?

Returns a the value associated with a given key.

func keyEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each key in the map table.

var count: Int

The number of key-value pairs in the map table.

