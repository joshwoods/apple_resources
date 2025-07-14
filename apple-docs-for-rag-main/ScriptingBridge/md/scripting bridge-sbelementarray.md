

- Scripting Bridge
-  SBElementArray 

Class

# SBElementArray

`SBElementArray` is subclass of `NSMutableArray` that manages collections of related SBObject objects. For example, when you ask the Finder for a list of disks, or ask iTunes for a list of playlists, you get the result back as an `SBElementArray` containing Scripting Bridge objects representing those items.

Mac Catalyst 13.0+macOS 10.5+

``` source
class SBElementArray
```

## Overview

`SBElementArray` defines methods beyond those of NSArray for obtaining individual objects. In addition to objectAtIndex:, `SBElementArray` also defines object(withName:), object(withID:), and object(atLocation:).

## Subclassing Notes

The `SBElementArray` class is not designed for subclassing.

## Topics

### Getting Objects in the Array

func object(withName: String) -> Any

Returns the object in the array with the given name.

func object(withID: Any) -> Any

Returns the object in the array with the given identifier.

func object(atLocation: Any) -> Any

Returns the object at the given location in the receiver.

### Getting the Referenced Array

func get() -> [Any]?

Forces evaluation of the receiver, causing the real object to be returned immediately.

### Filtering an Element Array

func array(byApplying: Selector) -> [Any]

Returns an array containing the results of sending the specified message to each object in the receiver.

func array(byApplying: Selector, with: Any) -> [Any]

Returns an array containing the results of sending the specified message to each object in the receiver.

## Relationships

### Inherits From

- NSMutableArray

### Conforms To

- CVarArg
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

