

- Foundation
- NSSet
-  enumerateObjects(options:using:) 

Instance Method

# enumerateObjects(options:using:)

Executes a given block using each object in the set, using the specified enumeration options.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func enumerateObjects(
    options opts: NSEnumerationOptions = [],
    using block: (Any, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`opts`  

A bitmask that specifies the options for the enumeration.

`block`  

The block to apply to elements in the set.

The block takes two arguments:

obj  
The element in the set.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the set. The `stop` argument is an out-only argument. You should only ever set this Boolean to true within the block.

## See Also

### Accessing Set Members

var allObjects: [Any]

An array containing the set’s members, or an empty array if the set has no members.

func anyObject() -> Any?

Returns one of the objects in the set, or `nil` if the set contains no objects.

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

func objects(passingTest: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns a set of objects that pass a test in a given block.

func objects(options: NSEnumerationOptions, passingTest: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns a set of objects that pass a test in a given block, using the specified enumeration options.

