

- Foundation
-  NSMutableDictionary 

Class

# NSMutableDictionary

A dynamic collection of objects associated with unique keys.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSMutableDictionary
```

## Overview

In Swift, you can use this type instead of a Dictionary variable in cases that require reference semantics.

The `NSMutableDictionary` class declares the programmatic interface to objects that manage mutable associations of keys and values. It adds modification operations to the basic operations it inherits from NSDictionary.

`NSMutableDictionary` is “toll-free bridged” with its Core Foundation counterpart, CFMutableDictionary. See Toll-Free Bridging for more information on toll-free bridging.

### Setting Values Using Subscripting

In addition to the provided instance methods, such as setObject(_:forKey:), you can access `NSDictionary` values by their keys using *subscripting*.

- Swift
- Objective-C

```
let value = "someValue"
mutableDictionary["someKey"] = value
```

```
id value = @"someValue";
mutableDictionary[@"someKey"] = value;
```

### Subclassing Notes

There should typically be little need to subclass `NSMutableDictionary`. If you do need to customize behavior, it is often better to consider composition rather than subclassing.

#### Methods to Override

In a subclass, you must override both of its primitive methods:

- setObject(_:forKey:)

- removeObject(forKey:)

You must also override the primitive methods of the NSDictionary class.

## Topics

### Creating and Initializing a Mutable Dictionary

init(capacity: Int)

Initializes a newly allocated mutable dictionary, allocating enough memory to hold `numItems` entries.

init()

Initializes a newly allocated mutable dictionary.

init(sharedKeySet: Any)

Creates a mutable dictionary which is optimized for dealing with a known set of keys.

### Adding Entries to a Mutable Dictionary

func setObject(Any, forKey: any NSCopying)

Adds a given key-value pair to the dictionary.

func setValue(Any?, forKey: String)

Adds a given key-value pair to the dictionary.

func addEntries(from: [AnyHashable : Any])

Adds to the receiving dictionary the entries from another dictionary.

func setDictionary([AnyHashable : Any])

Sets the contents of the receiving dictionary to entries in a given dictionary.

### Removing Entries From a Mutable Dictionary

func removeObject(forKey: Any)

Removes a given key and its associated value from the dictionary.

func removeAllObjects()

Empties the dictionary of its entries.

func removeObjects(forKeys: [Any])

Removes from the dictionary entries specified by elements in a given array.

### Initializers

convenience init!(OBEXHeadersData: Data!)

convenience init!(OBEXHeadersData: UnsafeRawPointer!, headersDataSize: Int)

init?(coder: NSCoder)

init?(contentsOfURL: URL)

### Instance Methods

func addApplicationParameterHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addAuthorizationChallengeHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addAuthorizationResponseHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addBodyHeader(UnsafeRawPointer!, length: UInt32, endOfBody: Bool) -> OBEXError

func addByteSequenceHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addConnectionIDHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addCountHeader(UInt32) -> OBEXError

func addDescriptionHeader(String!) -> OBEXError

func addHTTPHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addImageDescriptorHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addImageHandleHeader(String!) -> OBEXError

func addLengthHeader(UInt32) -> OBEXError

func addNameHeader(String!) -> OBEXError

func addObjectClassHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addTargetHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addTime4ByteHeader(UInt32) -> OBEXError

func addTimeISOHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addTypeHeader(String!) -> OBEXError

func addUserDefinedHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func addWhoHeader(UnsafeRawPointer!, length: UInt32) -> OBEXError

func getHeaderBytes() -> NSMutableData!

### Subscripts

subscript(Any) -> Any?

## Relationships

### Inherits From

- NSDictionary

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- ExpressibleByDictionaryLiteral
- Hashable
- NSCoding
- NSCopying
- NSFastEnumeration
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding
- Sequence

