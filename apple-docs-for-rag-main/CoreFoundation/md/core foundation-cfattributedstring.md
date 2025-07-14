

- Core Foundation
-  CFAttributedString 

Class

# CFAttributedString

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFAttributedString
```

## Overview

Instances of CFAttributedString manage character strings and associated sets of attributes (for example, font and kerning information) that apply to individual characters or ranges of characters in the string. CFAttributedString as defined in Core Foundation provides the basic container functionality, while higher levels provide definitions for standard attributes, their values, and additional behaviors involving these. CFAttributedString represents an immutable string—use CFMutableAttributedString to create and manage an attributed string that can be changed after it has been created.

CFAttributedString is not a “subclass” of CFString; that is, it does not respond to CFString function calls. CFAttributedString conceptually contains a CFString to which it applies attributes. This protects you from ambiguities caused by the semantic differences between simple and attributed string.

Attributes are identified by key/value pairs stored in CFDictionary objects. Keys must be CFString objects, while the corresponding values are CFType objects of an appropriate type. See the attribute constants in NSAttributedString Application Kit Additions Reference or NSAttributedString UIKit Additions Reference for standard attribute names.

Important

Attribute dictionaries set for an attributed string must always be created with kCFCopyStringDictionaryKeyCallBacks for their dictionary key callbacks and kCFTypeDictionaryValueCallBacks for their value callbacks; otherwise it’s an error.

CFAttributedString is “toll-free bridged” with its Foundation counterpart, NSAttributedString. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSAttributedString *` parameter, you can pass in a `CFAttributedStringRef`, and in a function where you see a `CFAttributedStringRef` parameter, you can pass in an NSAttributedString instance. This also applies to concrete subclasses of NSAttributedString. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating a CFAttributedString

func CFAttributedStringCreate(CFAllocator!, CFString!, CFDictionary!) -> CFAttributedString!

Creates an attributed string with specified string and attributes.

func CFAttributedStringCreateCopy(CFAllocator!, CFAttributedString!) -> CFAttributedString!

Creates an immutable copy of an attributed string.

func CFAttributedStringCreateWithSubstring(CFAllocator!, CFAttributedString!, CFRange) -> CFAttributedString!

Creates a sub-attributed string from the specified range.

func CFAttributedStringGetLength(CFAttributedString!) -> CFIndex

Returns the length of the attributed string in characters.

func CFAttributedStringGetString(CFAttributedString!) -> CFString!

Returns the string for an attributed string.

### Accessing Attributes

func CFAttributedStringGetAttribute(CFAttributedString!, CFIndex, CFString!, UnsafeMutablePointer&lt;CFRange>!) -> CFTypeRef!

Returns the value of a given attribute of an attributed string at a specified location.

func CFAttributedStringGetAttributes(CFAttributedString!, CFIndex, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

func CFAttributedStringGetAttributeAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFString!, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFTypeRef!

Returns the value of a given attribute of an attributed string at a specified location.

func CFAttributedStringGetAttributesAndLongestEffectiveRange(CFAttributedString!, CFIndex, CFRange, UnsafeMutablePointer&lt;CFRange>!) -> CFDictionary!

Returns the attributes of an attributed string at a specified location.

### Getting Attributed String Properties

func CFAttributedStringGetTypeID() -> CFTypeID

Returns the type identifier for the CFAttributedString opaque type.

## Relationships

### Inherited By

- CFMutableAttributedString

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

String Programming Guide for Core Foundation

Data Formatting Guide for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

