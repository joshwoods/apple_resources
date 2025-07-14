

- Foundation
- NSHashTable
-  objectEnumerator() 

Instance Method

# objectEnumerator()

Returns an enumerator object that lets you access each object in the hash table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func objectEnumerator() -> NSEnumerator
```

## Return Value

An enumerator object that lets you access each object in the hash table.

## Discussion

The following code fragment illustrates how you can use this method.

```
NSEnumerator *enumerator = [myHashTable objectEnumerator];
id value;

while ((value = [enumerator nextObject])) {
    /* code that acts on the hash table's values */
}
```

### Special Considerations

It is more efficient to use the fast enumeration protocol (see NSFastEnumeration).

## See Also

### Accessing Content

var anyObject: ObjectType?

One of the objects in the hash table.

var allObjects: [ObjectType]

The hash table’s members.

var setRepresentation: Set&lt;AnyHashable>

A set that contains the hash table’s members.

var count: Int

The number of elements in the hash table.

func contains(ObjectType?) -> Bool

Returns a Boolean value that indicates whether the hash table contains a given object.

func member(ObjectType?) -> ObjectType?

Determines whether the hash table contains a given object, and returns that object if it is present

