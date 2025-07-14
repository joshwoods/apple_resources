

- Foundation
-  NSArray 

Class

# NSArray

A static ordered collection of objects.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSArray
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

You can use this type in Swift instead of an Array constant in cases that require reference semantics.

`NSArray` and its subclass NSMutableArray manage ordered collections of objects called **arrays**. `NSArray` creates static arrays, and `NSMutableArray` creates dynamic arrays. You can use arrays when you need an ordered collection of objects.

`NSArray` is “toll-free bridged” with its Core Foundation counterpart, doc://com.apple.documentation/documentation/corefoundation/cfarray-s28. See Toll-Free Bridging for more information on toll-free bridging.

### Creating NSArray Objects Using Array Literals

In addition to the provided initializers, such as initWithObjects:, you can create an `NSArray` object using an *array literal*.

- Swift
- Objective-C

```
let array: NSArray = [someObject, "Hello, World!", 42]
```

```
NSArray *array = @[someObject, @"Hello, World!", @42];
```

In Objective-C, the compiler generates code that makes an underlying call to the init(objects:count:) method.

```
id objects[] = { someObject, @"Hello, World!", @42 };
NSUInteger count = sizeof(objects) / sizeof(id);
NSArray *array = [NSArray arrayWithObjects:objects
                                     count:count];
```

You should not terminate the list of objects with `nil` when using this literal syntax, and in fact `nil` is an invalid value. For more information about object literals in Objective-C, see Working with Objects in Programming with Objective-C.

In Swift, the `NSArray` class conforms to the `ArrayLiteralConvertible` protocol, which allows it to be initialized with array literals. For more information about object literals in Swift, see Literal Expression in The Swift Programming Language (Swift 4.1).

### Accessing Values Using Subscripting

In addition to the provided instance methods, such as object(at:), you can access `NSArray` values by their indexes using *subscripting*.

- Swift
- Objective-C

```
let value = array[3]
```

```
id value = array[3];
```

### Subclassing Notes

There is typically little reason to subclass `NSArray`. The class does well what it is designed to do—maintain an ordered collection of objects. But there are situations where a custom `NSArray` object might come in handy. Here are a few possibilities:

- Changing how `NSArray` stores the elements of its collection. You might do this for performance reasons or for better compatibility with legacy code.

- Acquiring more information about what is happening to the collection (for example, statistics gathering).

#### Methods to Override

Any subclass of `NSArray` *must* override the primitive instance methods count and object(at:). These methods must operate on the backing store that you provide for the elements of the collection. For this backing store you can use a static array, a standard `NSArray` object, or some other data type or mechanism. You may also choose to override, partially or fully, any other `NSArray` method for which you want to provide an alternative implementation.

You might want to implement an initializer for your subclass that is suited to the backing store that the subclass is managing. If you do, your initializer must invoke one of the designated initializers of the `NSArray` class, either init() or init(objects:count:). The `NSArray` class adopts the NSCopying, NSMutableCopying, and NSCoding protocols; custom subclasses of `NSArray` should override the methods in these protocols as necessary.

Remember that `NSArray` is the public interface for a class cluster and what this entails for your subclass. You must provide the storage for your subclass and implement the primitive methods that directly act on that storage.

#### Alternatives to Subclassing

Before making a custom subclass of `NSArray`, investigate NSPointerArray and the corresponding Core Foundation type, doc://com.apple.documentation/documentation/corefoundation/cfarray-s28. Because `NSArray` and `CFArray` are “toll-free bridged,” you can substitute a `CFArray` object for a `NSArray` object in your code (with appropriate casting). Although they are corresponding types, `CFArray` and `NSArray` do not have identical interfaces or implementations, and you can sometimes do things with `CFArray` that you cannot easily do with `NSArray`. For example, `CFArray` provides a set of callbacks, some of which are for implementing custom retain-release behavior. If you specify `NULL` implementations for these callbacks, you can easily get a non-retaining array.

If the behavior you want to add supplements that of the existing class, you could write a category on `NSArray`. Keep in mind, however, that this category will be in effect for all instances of `NSArray` that you use, and this might have unintended consequences. Alternatively, you could use composition to achieve the desired behavior.

## Topics

### Creating an Array

init?(contentsOfURL: URL)

Creates and returns an array containing the contents specified by a given URL.

convenience init(object: Any)

Creates and returns an array containing a given object.

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns an array that includes a given number of objects from a given C array.

### Initializing an Array

init()

Initializes a newly allocated array.

convenience init(array: [Any])

Initializes a newly allocated array by placing in it the objects contained in a given array.

convenience init(array: [Any], copyItems: Bool)

Initializes a newly allocated array using `anArray` as the source of data objects for the array.

convenience init?(contentsOfFile: String)

Initializes a newly allocated array with the contents of the file specified by a given path.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated array with the contents of the location specified by a given URL.

init(objects: UnsafePointer&lt;AnyObject>?, count: Int)

Initializes a newly allocated array to include a given number of objects from a given C array.

### Querying an Array

func contains(Any) -> Bool

Returns a Boolean value that indicates whether a given object is present in the array.

var count: Int

The number of objects in the array.

var firstObject: Any?

The first object in the array.

var lastObject: Any?

The last object in the array.

func object(at: Int) -> Any

Returns the object located at the specified index.

subscript(Int) -> Any

Returns the object at the specified index.

func objects(at: IndexSet) -> [Any]

Returns an array containing the objects in the array at the indexes specified by a given index set.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array.

func reverseObjectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each object in the array, in reverse order.

### Finding Objects in an Array

func index(of: Any) -> Int

Returns the lowest index whose corresponding array value is equal to a given object.

func index(of: Any, in: NSRange) -> Int

Returns the lowest index within a specified range whose corresponding array value is equal to a given object .

func indexOfObjectIdentical(to: Any) -> Int

Returns the lowest index whose corresponding array value is identical to a given object.

func indexOfObjectIdentical(to: Any, in: NSRange) -> Int

Returns the lowest index within a specified range whose corresponding array value is equal to a given object .

func indexOfObject(passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of the first object in the array that passes a test in a given block.

func indexOfObject(options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index of an object in the array that passes a test in a given block for a given set of enumeration options.

func indexOfObject(at: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Int

Returns the index, from a given set of indexes, of the first object in the array that passes a test in a given block for a given set of enumeration options.

func indexesOfObjects(passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes of objects in the array that pass a test in a given block.

func indexesOfObjects(options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes of objects in the array that pass a test in a given block for a given set of enumeration options.

func indexesOfObjects(at: IndexSet, options: NSEnumerationOptions, passingTest: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> IndexSet

Returns the indexes, from a given set of indexes, of objects in the array that pass a test in a given block for a given set of enumeration options.

func index(of: Any, inSortedRange: NSRange, options: NSBinarySearchingOptions, usingComparator: (Any, Any) -> ComparisonResult) -> Int

Returns the index, within a specified range, of an object compared with elements in the array using a given `NSComparator` block.

### Sending Messages to Elements

func enumerateObjects((Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given closure or block using each object in the array, starting with the first object and continuing through the array to the last object.

func enumerateObjects(options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given closure or block using each object in the array with the specified options.

func enumerateObjects(at: IndexSet, options: NSEnumerationOptions, using: (Any, Int, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Executes a given block using the objects in the array at the specified indexes.

### Comparing Arrays

func firstObjectCommon(with: [Any]) -> Any?

Returns the first object contained in the receiving array that’s equal to an object in another given array.

func isEqual(to: [Any]) -> Bool

Compares the receiving array to another array.

### Deriving New Arrays

func adding(Any) -> [Any]

Returns a new array that is a copy of the receiving array with a given object added to the end.

func addingObjects(from: [Any]) -> [Any]

Returns a new array that is a copy of the receiving array with the objects contained in another array added to the end.

func filtered(using: NSPredicate) -> [Any]

Evaluates a given predicate against each object in the receiving array and returns a new array containing the objects for which the predicate returns true.

func subarray(with: NSRange) -> [Any]

Returns a new array containing the receiving array’s elements that fall within the limits specified by a given range.

### Sorting

var sortedArrayHint: Data

Analyzes the array and returns a “hint” that speeds the sorting of the array when the hint is supplied to sortedArray(_:context:hint:).

func sortedArray((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?) -> [Any]

Returns a new array that lists the receiving array’s elements in ascending order as defined by the comparison function `comparator`.

func sortedArray((Any, Any, UnsafeMutableRawPointer?) -> Int, context: UnsafeMutableRawPointer?, hint: Data?) -> [Any]

Returns a new array that lists the receiving array’s elements in ascending order as defined by the comparison function `comparator`.

func sortedArray(using: [NSSortDescriptor]) -> [Any]

Returns a copy of the receiving array sorted as specified by a given array of sort descriptors.

func sortedArray(using: Selector) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given selector.

func sortedArray(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

func sortedArray(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array that lists the receiving array’s elements in ascending order, as determined by the comparison method specified by a given `NSComparator` block.

typealias Comparator

Defines the signature for a block object used for comparison operations.

### Working with String Elements

func componentsJoined(by: String) -> String

Constructs and returns an `NSString` object that is the result of interposing a given separator between the elements of the array.

### Creating a Description

var description: String

func description(withLocale: Any?) -> String

func description(withLocale: Any?, indent: Int) -> String

### Storing Arrays

func write(toFile: String, atomically: Bool) -> Bool

Writes the contents of the array to a file at a given path.

func write(to: URL, atomically: Bool) -> Bool

Writes the contents of the array to the location specified by a given URL.

### Collecting Paths

func pathsMatchingExtensions([String]) -> [String]

Returns an array containing all the pathname elements in the receiving array that have filename extensions from a given array.

### Key-Value Observing

func addObserver(NSObject, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String)

Raises an exception.

func removeObserver(NSObject, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String, context: UnsafeMutableRawPointer?)

Raises an exception.

func addObserver(NSObject, toObjectsAt: IndexSet, forKeyPath: String, options: NSKeyValueObservingOptions, context: UnsafeMutableRawPointer?)

Registers an observer to receive key value observer notifications for the specified key-path relative to the objects at the indexes.

func removeObserver(NSObject, fromObjectsAt: IndexSet, forKeyPath: String)

Removes `anObserver` from all key value observer notifications associated with the specified `keyPath` relative to the array’s objects at `indexes`.

### Key-Value Coding

func setValue(Any?, forKey: String)

Invokes setValue(_:forKey:) on each of the array’s items using the specified `value` and `key`.

func value(forKey: String) -> Any

Returns an array containing the results of invoking value(forKey:) using `key` on each of the array’s objects.

### Randomly Shuffling an Array

func shuffled() -> [Any]

Returns a new array that lists this array’s elements in a random order.

func shuffled(using: GKRandomSource) -> [Any]

Returns a new array that lists this array’s elements in a random order, using the specified random source.

### Comparing with Another Array

class NSOrderedCollectionDifference

An object representing the difference between two ordered collections.

struct NSOrderedCollectionDifferenceCalculationOptions

Constants that specify the options to use when creating an ordered collection difference.

### New Methods

init?(coder: NSCoder)

### Constants

struct NSBinarySearchingOptions

Options for searches and insertions using index(of:inSortedRange:options:usingComparator:).

### Initializers

convenience init(array: NSArray)

convenience init(contentsOfURL: URL, error: ()) throws

convenience init(objects: Any...)

### Instance Methods

func write(to: URL) throws

### Default Implementations

ExpressibleByArrayLiteral Implementations

Sequence Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableArray

### Conforms To

- CKRecordValue
- CKRecordValueProtocol
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

