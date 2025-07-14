

- Core Foundation
-  CFCharacterSet 

Class

# CFCharacterSet

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFCharacterSet
```

## Overview

A CFCharacterSet object represents a set of Unicode compliant characters. CFString uses CFCharacterSet objects to group characters together for searching operations, so that they can find any of a particular set of characters during a search. The two opaque types, CFCharacterSet and CFMutableCharacterSet, define the interface for static and dynamic character sets, respectively. The objects you create using these opaque types are referred to as character set objects (and when no confusion will result, merely as character sets).

CFCharacterSet’s principal function, CFCharacterSetIsCharacterMember(_:_:), provides the basis for all other functions in its interface. You create a character set using one of the `CFCharacterSetCreate...` functions. You may also use any one of the predefined character sets using the CFCharacterSetGetPredefined(_:) function.

CFCharacterSet is “toll-free bridged” with its Cocoa Foundation counterpart, NSCharacterSet. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSCharacterSet *` parameter, you can pass in a `CFCharacterSetRef`, and in a function where you see a `CFCharacterSetRef` parameter, you can pass in an NSCharacterSet instance. This capability also applies to concrete subclasses of NSCharacterSet. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating Character Sets

func CFCharacterSetCreateCopy(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new character set with the values from a given character set.

func CFCharacterSetCreateInvertedSet(CFAllocator!, CFCharacterSet!) -> CFCharacterSet!

Creates a new immutable character set that is the invert of the specified character set.

func CFCharacterSetCreateWithCharactersInRange(CFAllocator!, CFRange) -> CFCharacterSet!

Creates a new character set with the values from the given range of Unicode characters.

func CFCharacterSetCreateWithCharactersInString(CFAllocator!, CFString!) -> CFCharacterSet!

Creates a new character set with the values in the given string.

func CFCharacterSetCreateWithBitmapRepresentation(CFAllocator!, CFData!) -> CFCharacterSet!

Creates a new immutable character set with the bitmap representation specified by given data.

### Getting Predefined Character Sets

func CFCharacterSetGetPredefined(CFCharacterSetPredefinedSet) -> CFCharacterSet!

Returns a predefined character set.

### Querying Character Sets

func CFCharacterSetCreateBitmapRepresentation(CFAllocator!, CFCharacterSet!) -> CFData!

Creates a new immutable data with the bitmap representation from the given character set.

func CFCharacterSetHasMemberInPlane(CFCharacterSet!, CFIndex) -> Bool

Reports whether or not a character set contains at least one member character in the specified plane.

func CFCharacterSetIsCharacterMember(CFCharacterSet!, UniChar) -> Bool

Reports whether or not a given Unicode character is in a character set.

func CFCharacterSetIsLongCharacterMember(CFCharacterSet!, UTF32Char) -> Bool

Reports whether or not a given UTF-32 character is in a character set.

func CFCharacterSetIsSupersetOfSet(CFCharacterSet!, CFCharacterSet!) -> Bool

Reports whether or not a character set is a superset of another set.

### Getting the Character Set Type Identifier

func CFCharacterSetGetTypeID() -> CFTypeID

Returns the type identifier of the CFCharacterSet opaque type.

### Data Types

enum CFCharacterSetPredefinedSet

Defines a predefined character set.

### Constants

Predefined CFCharacterSet Selector Values

Identifiers for the available predefined CFCharacterSet objects.

## Relationships

### Inherited By

- CFMutableCharacterSet

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

String Programming Guide for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

