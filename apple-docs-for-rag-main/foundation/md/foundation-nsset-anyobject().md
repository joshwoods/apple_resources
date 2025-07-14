

- Foundation
- NSSet
-  anyObject() 

Instance Method

# anyObject()

Returns one of the objects in the set, or `nil` if the set contains no objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func anyObject() -> Any?
```

## Return Value

One of the objects in the set, or `nil` if the set contains no objects. The object returned is chosen at the set’s convenience—the selection is not guaranteed to be random.

## See Also

### Accessing Set Members

var allObjects: [Any]

An array containing the set’s members, or an empty array if the set has no members.

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the set.

func filtered(using: NSPredicate) -> Set&lt;AnyHashable>

Evaluates a given predicate against each object in the receiving set and returns a new set containing the objects for which the predicate returns true.

func member(Any) -> Any?

Determines whether a given object is present in the set, and returns that object if it is.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the set.

func enumerateObjects((Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the set.

func enumerateObjects(options: NSEnumerationOptions, using: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the set, using the specified enumeration options.

func objects(passingTest: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns a set of objects that pass a test in a given block.

func objects(options: NSEnumerationOptions, passingTest: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns a set of objects that pass a test in a given block, using the specified enumeration options.

