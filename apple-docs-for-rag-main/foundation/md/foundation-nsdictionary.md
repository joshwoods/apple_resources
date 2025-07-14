

- Foundation
-  NSDictionary 

Class

# NSDictionary

A static collection of objects associated with unique keys.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSDictionary
```

## Mentioned in 

Implementing Handoff in Your App

## Overview

You can use this type in Swift instead of a Dictionary in cases that require reference semantics.

The `NSDictionary` class declares the programmatic interface to objects that manage immutable associations of keys and values. For example, an interactive form could be represented as a dictionary, with the field names as keys, corresponding to user-entered values.

Use this class or its subclass NSMutableDictionary when you need a convenient and efficient way to retrieve data associated with an arbitrary key. `NSDictionary` creates static dictionaries, and `NSMutableDictionary` creates dynamic dictionaries. (For convenience, the term *dictionary* refers to any instance of one of these classes without specifying its exact class membership.)

A key-value pair within a dictionary is called an entry. Each entry consists of one object that represents the key and a second object that is that key’s value. Within a dictionary, the keys are unique. That is, no two keys in a single dictionary are equal (as determined by isEqual(_:)). In general, a key can be any object (provided that it conforms to the `NSCopying` protocol—see below), but note that when using key-value coding the key must be a string (see Accessing Object Properties). Neither a key nor a value can be `nil`; if you need to represent a null value in a dictionary, you should use NSNull.

`NSDictionary` is “toll-free bridged” with its Core Foundation counterpart, doc://com.apple.documentation/documentation/corefoundation/cfdictionary-rum. See Toll-Free Bridging for more information on toll-free bridging.

### Creating NSDictionary Objects Using Dictionary Literals

In addition to the provided initializers, such as init(objects:forKeys:), you can create an `NSDictionary` object using a *dictionary literal*.

- Swift
- Objective-C

```
let dictionary: NSDictionary = [
    "anObject" : someObject,
    "helloString" : "Hello, World!",
    "magicNumber" : 42,
    "aValue" : someValue
]
```

```
NSDictionary *dictionary = @{
       @"anObject" : someObject,
    @"helloString" : @"Hello, World!",
    @"magicNumber" : @42,
         @"aValue" : someValue
};
```

In Objective-C, the compiler generates code that makes an underlying call to the dictionaryWithObjects:forKeys:count: method.

```
id objects[] = { someObject, @"Hello, World!", @42, someValue };
id keys[] = { @"anObject", @"helloString", @"magicNumber", @"aValue" };
NSUInteger count = sizeof(objects) / sizeof(id);
NSDictionary *dictionary = [NSDictionary dictionaryWithObjects:objects
                                                       forKeys:keys
                                                         count:count];
```

Unlike dictionaryWithObjectsAndKeys: and other initializers, dictionary literals specify entries in key-value order. You should not terminate the list of objects with `nil` when using this literal syntax, and in fact `nil` is an invalid value. For more information about object literals in Objective-C, see Working with Objects in Programming with Objective-C.

In Swift, the `NSDictionary` class conforms to the `DictionaryLiteralConvertible` protocol, which allows it to be initialized with dictionary literals. For more information about object literals in Swift, see Literal Expression in The Swift Programming Language (Swift 4.1).

### Accessing Values Using Subscripting

In addition to the provided instance methods, such as object(forKey:), you can access `NSDictionary` values by their keys using *subscripting*.

- Swift
- Objective-C

```
let value = dictionary["helloString"]
```

```
id value = dictionary[@"helloString"];
```

### Enumerating Entries Using for-in Loops

In addition to the provided instance methods, such as enumerateKeysAndObjects(_:), you can enumerate `NSDictionary` entries using *for-in loops*.

- Swift
- Objective-C

```
for (key, value) in dictionary {
    print("Value: \(value) for key: \(key)")
}
```

```
for (NSString *key in dictionary) {
    id value = dictionary[key];
    NSLog(@"Value: %@ for key: %@", value, key);
}
```

In Objective-C, `NSDictionary` conforms to the NSFastEnumeration protocol.

In Swift, `NSDictionary` conforms to the `SequenceType` protocol.

### Subclassing Notes

You generally shouldn’t need to subclass `NSDictionary`. Custom behavior can usually be achieved through composition rather than subclassing.

#### Methods to Override

If you do need to subclass `NSDictionary`, take into account that it is a Class cluster. Any subclass must override the following primitive methods:

- init(objects:forKeys:count:)

- count

- object(forKey:)

- keyEnumerator()

The other methods of `NSDictionary` operate by invoking one or more of these primitives. The non-primitive methods provide convenient ways of accessing multiple entries at once.

#### Alternatives to Subclassing

Before making a custom class of `NSDictionary`, investigate NSMapTable and the corresponding Core Foundation type, CFDictionary. Because `NSDictionary` and `CFDictionary` are “toll-free bridged,” you can substitute a `CFDictionary` object for a `NSDictionary` object in your code (with appropriate casting). Although they are corresponding types, `CFDictionary` and `NSDictionary` do not have identical interfaces or implementations, and you can sometimes do things with `CFDictionary` that you cannot easily do with `NSDictionary`.

If the behavior you want to add supplements that of the existing class, you could write a category on `NSDictionary`. Keep in mind, however, that this category will be in effect for all instances of `NSDictionary` that you use, and this might have unintended consequences. Alternatively, you could use composition to achieve the desired behavior.

## Topics

### Creating an Empty Dictionary

init()

Initializes a newly allocated dictionary.

### Creating a Dictionary from Objects and Keys

convenience init(objects: [Any], forKeys: [any NSCopying])

Initializes a newly allocated dictionary with key-value pairs constructed from the provided arrays of keys and objects.

init(objects: UnsafePointer&lt;AnyObject>?, forKeys: UnsafePointer&lt;any NSCopying>?, count: Int)

Initializes a newly allocated dictionary with the specified number of key-value pairs constructed from the provided C arrays of keys and objects.

convenience init(object: Any, forKey: any NSCopying)

Creates a dictionary containing a given key and value.

### Creating a Dictionary from Another Dictionary

convenience init(dictionary: [AnyHashable : Any])

Initializes a newly allocated dictionary by placing in it the keys and values contained in another given dictionary.

convenience init(dictionary: [AnyHashable : Any], copyItems: Bool)

Initializes a newly allocated dictionary using the objects contained in another given dictionary.

### Creating a Dictionary from an External Source

init?(contentsOfURL: URL)

Creates a dictionary using the keys and values found in a resource specified by a given URL.

Deprecated

convenience init(contentsOfURL: URL, error: ()) throws

Initializes a newly allocated dictionary using the keys and values found at a given URL.

convenience init?(contentsOfURL: URL)

Initializes a newly allocated dictionary using the keys and values found at a given URL.

Deprecated

convenience init?(contentsOfFile: String)

Initializes a newly allocated dictionary using the keys and values found in a file at a given path.

### Creating a Dictionary from an NSCoder

init?(coder: NSCoder)

Creates a dictionary initialized from data in the provided unarchiver.

### Creating Key Sets for Shared-Key Optimized Dictionaries

class func sharedKeySet(forKeys: [any NSCopying]) -> Any

Creates a shared key set object for the specified keys.

### Counting Entries

var count: Int

The number of entries in the dictionary.

### Comparing Dictionaries

func isEqual(to: [AnyHashable : Any]) -> Bool

Returns a Boolean value that indicates whether the contents of the receiving dictionary are equal to the contents of another given dictionary.

### Accessing Keys and Values

var allKeys: [Any]

A new array containing the dictionary’s keys, or an empty array if the dictionary has no entries.

func allKeys(for: Any) -> [Any]

Returns a new array containing the keys corresponding to all occurrences of a given object in the dictionary.

var allValues: [Any]

A new array containing the dictionary’s values, or an empty array if the dictionary has no entries.

func value(forKey: String) -> Any?

Returns the value associated with a given key.

func objects(forKeys: [Any], notFoundMarker: Any) -> [Any]

Returns as a static array the set of objects from the dictionary that corresponds to the specified keys.

func object(forKey: Any) -> Any?

Returns the value associated with a given key.

subscript(any NSCopying) -> Any?

Returns the value associated with a given key.

subscript(Any) -> Any?

Accesses the value associated with a given key.

### Enumerating Dictionaries

func keyEnumerator() -> NSEnumerator

Provides an enumerator to access the keys in the dictionary.

func objectEnumerator() -> NSEnumerator

Returns an enumerator object that lets you access each value in the dictionary.

func enumerateKeysAndObjects((Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary.

func enumerateKeysAndObjects(options: NSEnumerationOptions, using: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Applies a given block object to the entries of the dictionary, with options specifying how the enumeration is performed.

func makeIterator() -> NSDictionary.Iterator

Returns an iterator over the elements of this sequence.

### Sorting Dictionaries

func keysSortedByValue(using: Selector) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values.

func keysSortedByValue(comparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using a given comparator block.

func keysSortedByValue(options: NSSortOptions, usingComparator: (Any, Any) -> ComparisonResult) -> [Any]

Returns an array of the dictionary’s keys, in the order they would be in if the dictionary were sorted by its values using a given comparator block and a specified set of options.

### Filtering Dictionaries

func keysOfEntries(passingTest: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns the set of keys whose corresponding value satisfies a constraint described by a block object.

func keysOfEntries(options: NSEnumerationOptions, passingTest: (Any, Any, UnsafeMutablePointer&lt;ObjCBool>) -> Bool) -> Set&lt;AnyHashable>

Returns the set of keys whose corresponding value satisfies a constraint described by a block object.

### Storing Dictionaries

func write(to: URL) throws

Writes a property list representation of the contents of the dictionary to a given URL.

func write(to: URL, atomically: Bool) -> Bool

Writes a property list representation of the contents of the dictionary to a given URL.

Deprecated

func write(toFile: String, atomically: Bool) -> Bool

Writes a property list representation of the contents of the dictionary to a given path.

Deprecated

### Accessing File Attributes

These convenience methods are for use with dictionaries returned by the FileManager method attributesOfItem(atPath:), and allow you to access POSIX and HFS attributes for files and directories.

func fileSize() -> UInt64

Returns the file’s size, in bytes.

func fileType() -> String?

Returns the file type.

func fileCreationDate() -> Date?

Returns the file’s creation date.

func fileModificationDate() -> Date?

Returns file’s modification date.

func filePosixPermissions() -> Int

Returns the file’s POSIX permissions.

func fileOwnerAccountID() -> NSNumber?

Returns the file’s owner account ID.

func fileOwnerAccountName() -> String?

Returns the file’s owner account name.

func fileGroupOwnerAccountID() -> NSNumber?

Returns file’s group owner account ID.

func fileGroupOwnerAccountName() -> String?

Returns the file’s group owner account name.

func fileExtensionHidden() -> Bool

Returns a Boolean value indicating whether the file hides its extension.

func fileIsImmutable() -> Bool

Returns a Boolean value indicating whether the file is immutable.

func fileIsAppendOnly() -> Bool

Returns a Boolean value indicating whether the file is append only.

func fileSystemFileNumber() -> Int

Returns the filesystem file number.

func fileSystemNumber() -> Int

Returns the filesystem number.

func fileHFSTypeCode() -> OSType

Returns file’s HFS type code.

func fileHFSCreatorCode() -> OSType

Returns the file’s HFS creator code.

### Describing a Dictionary

var description: String

var descriptionInStringsFileFormat: String

func description(withLocale: Any?) -> String

func description(withLocale: Any?, indent: Int) -> String

### Initializers

convenience init(dictionary: NSDictionary)

### Default Implementations

Sequence Implementations

## Relationships

### Inherits From

- NSObject

### Inherited By

- NSMutableDictionary

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- ExpressibleByDictionaryLiteral
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSFetchRequestResult
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Sequence

