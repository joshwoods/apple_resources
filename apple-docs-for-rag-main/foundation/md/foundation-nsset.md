

- Foundation
-  NSSet 

Class

# NSSet

A static, unordered collection of unique objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSSet
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

The NSSet, NSMutableSet, and NSCountedSet classes declare the programmatic interface to an unordered collection of objects.

NSSet declares the programmatic interface for static sets of distinct objects. You establish a static set’s entries when it’s created, and can’t modify the entries after that. NSMutableSet, on the other hand, declares a programmatic interface for dynamic sets of distinct objects. A dynamic — or mutable — set allows the addition and deletion of entries at any time, automatically allocating memory as needed.

Use sets as an alternative to arrays when the order of elements isn’t important and you need to consider performance in testing whether the set contains an object. With an array, testing for membership is slower than with sets.

NSSet is “toll-free bridged” with its Core Foundation counterpart, CFSet. See Toll-Free Bridging for more information on toll-free bridging.

In Swift, use this class instead of a Set constant in cases where you require reference semantics.

### Subclassing Notes

There should be little need of subclassing. If you need to customize behavior, it’s often better to consider composition instead of subclassing.

#### Methods to Override

In a subclass, you must override all of its primitive methods:

- count

- member(_:)

- objectEnumerator()

#### Alternatives to Subclassing

Before making a custom class of NSSet, investigate NSHashTable and the corresponding Core Foundation type, doc://com.apple.documentation/documentation/corefoundation/cfset-rgt. Because NSSet and doc://com.apple.documentation/documentation/corefoundation/cfset-rgt are “toll-free bridged,” you can substitute a doc://com.apple.documentation/documentation/corefoundation/cfset-rgt object for a NSSet object in your code (with appropriate casting). Although they’re corresponding types, doc://com.apple.documentation/documentation/corefoundation/cfset-rgt and NSSet don’t have identical interfaces or implementations, and you can sometimes do things with doc://com.apple.documentation/documentation/corefoundation/cfset-rgt that you can’t easily do with NSSet.

If the behavior you want to add supplements that of the existing class, you could write a category on NSSet. Keep in mind, however, that this category affects all instances of NSSet that you use, and this might have unintended consequences. Alternatively, you could use composition to achieve the desired behavior.

## Topics

### Creating a Set

convenience init(object: Any)

Creates and returns a set that contains a single given object.

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns a set containing a specified number of objects from a given C array of objects.

func adding(Any) -> Set&lt;AnyHashable>

Returns a new set formed by adding a given object to the receiving set.

func addingObjects(from: Set&lt;AnyHashable>) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given set to the receiving set.

func addingObjects(from: [Any]) -> Set&lt;AnyHashable>

Returns a new set formed by adding the objects in a given array to the receiving set.

### Initializing a Set

convenience init(array: [Any])

Initializes a newly allocated set with the objects that are contained in a given array.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated set with a specified number of objects from a given C array of objects.

convenience init(set: Set&lt;AnyHashable>)

Initializes a newly allocated set and adds to it objects from another given set.

convenience init(set: Set&lt;AnyHashable>, copyItems: Bool)

Initializes a newly allocated set and adds to it members of another given set.

init()

Initializes a newly allocated set.

### Counting Entries

var count: Int

The number of members in the set.

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

func enumerateObjects(options: NSEnumerationOptions, using: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using each object in the set, using the specified enumeration options.

func objects(passingTest: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns a set of objects that pass a test in a given block.

func objects(options: NSEnumerationOptions, passingTest: (Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns a set of objects that pass a test in a given block, using the specified enumeration options.

### Comparing Sets

func isSubset(of: Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether every object in the receiving set is also present in another given set.

func intersects(Set&lt;AnyHashable>) -> Bool

Returns a Boolean value that indicates whether at least one object in the receiving set is also present in another given set.

func isEqual(to: Set&lt;AnyHashable>) -> Bool

Compares the receiving set to another set.

func value(forKey: String) -> Any

Return a set containing the results of invoking `valueForKey:` on each of the receiving set’s members.

func setValue(Any?, forKey: String)

Invokes `setValue:forKey:` on each of the set’s members.

### Creating a Sorted Array

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns an array of the set’s content sorted as specified by a given array of sort descriptors.

### Key-Value Observing

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

### Describing a Set

var description: String

func description(withLocale: Any?) -> String

### Initializers

init?(coder: NSCoder)

convenience init(collectionViewIndexPath: IndexPath)

convenience init(collectionViewIndexPaths: [IndexPath])

convenience init(objects: Any...)

convenience init(set: NSSet)

### Instance Methods

func enumerateIndexPaths(options: NSEnumerationOptions, using: (IndexPath, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

### Default Implementations

Sequence Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableSet

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- ExpressibleByArrayLiteral
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Sequence

