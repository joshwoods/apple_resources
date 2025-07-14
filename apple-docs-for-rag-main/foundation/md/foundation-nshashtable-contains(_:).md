

- Foundation
- NSHashTable
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the hash table contains a given object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ anObject: ObjectType?) -> Bool
```

## Parameters 

`anObject`  

The object to test for membership in the hash table.

## Return Value

true if the hash table contains `anObject`, otherwise false.

## Discussion

The equality test used depends on the personality option selected. For instance, choosing the objectPersonality option will use `isEqual:` to determine equality. See NSPointerFunctions.Options for more information on personality options and their corresponding equality tests.

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

func member(ObjectType?) -> ObjectType?

Determines whether the hash table contains a given object, and returns that object if it is present

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the hash table.

