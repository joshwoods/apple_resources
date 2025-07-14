

- Core Foundation
-  CFPropertyList 

Type Alias

# CFPropertyList

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFPropertyList = CFTypeRef
```

## Overview

CFPropertyList provides functions that convert property list objects to and from several serialized formats such as XML. The CFPropertyList type that denotes CFPropertyList objects is an abstract type for property list objects. Depending on the contents of the XML data used to create the property list, `CFPropertyListRef` can be any of the property list objects: CFData, CFString, CFArray, CFDictionary, CFDate, CFBoolean, and CFNumber. Note that if you use a property list to generate XML, the keys of any dictionaries in the property list must be CFString objects.

It is important to understand that CFPropertyList provides an abstraction for all the property list types—you can think of CFPropertyList in object-oriented terms as being the superclass of CFString, CFNumber, CFDictionary, and so on. When a Core Foundation function returns a `CFPropertyListRef`, it means that the value may be any of the property list types. For example, CFPreferencesCopyAppValue(_:_:) returns a `CFPropertyListRef`. This means that the value returned can be a CFString object, a CFNumber object, a CFDictionary object, and so on again. You can use CFGetTypeID(_:) to determine what type of object a property list value is.

You use one of the `CFPropertyListCreate...` functions to create a property list object given an existing property list object, raw XML data (as in a file), or a stream. You can also convert a property list object to XML using the CFPropertyListCreateXMLData(_:_:) function. You use the CFPropertyListWriteToStream(_:_:_:_:) function to write a property list to an output stream, and validate a property list object using the CFPropertyListIsValid(_:_:) function. CFPropertyList properly takes care of endian issues—a property list (whether represented by a stream, XML, or a CFData object) created on a PowerPC-based Macintosh is correctly interpreted on an Intel-based Macintosh, and vice versa.

For code examples illustrating how to read and write property list files, see Property List Programming Topics for Core Foundation and in particular Saving and Restoring Property Lists.

## Topics

### Creating a Property List

func CFPropertyListCreateWithData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list from a given CFData object.

func CFPropertyListCreateWithStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFPropertyList>!

Create and return a property list with a CFReadStream input.

func CFPropertyListCreateDeepCopy(CFAllocator!, CFPropertyList!, CFOptionFlags) -> CFPropertyList!

Recursively creates a copy of a given property list.

func CFPropertyListCreateFromXMLData(CFAllocator!, CFData!, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using the specified XML or binary property list data.

Deprecated

func CFPropertyListCreateFromStream(CFAllocator!, CFReadStream!, CFIndex, CFOptionFlags, UnsafeMutablePointer&lt;CFPropertyListFormat>!, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> Unmanaged&lt;CFPropertyList>!

Creates a property list using data from a stream.

Deprecated

### Exporting a Property List

func CFPropertyListCreateData(CFAllocator!, CFPropertyList!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> Unmanaged&lt;CFData>!

Returns a CFData object containing a serialized representation of a given property list in a specified format.

func CFPropertyListWrite(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, CFOptionFlags, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>!) -> CFIndex

Write the bytes of a serialized property list out to a stream.

func CFPropertyListCreateXMLData(CFAllocator!, CFPropertyList!) -> Unmanaged&lt;CFData>!

Creates an XML representation of the specified property list.

Deprecated

func CFPropertyListWriteToStream(CFPropertyList!, CFWriteStream!, CFPropertyListFormat, UnsafeMutablePointer&lt;Unmanaged&lt;CFString>?>!) -> CFIndex

Writes the bytes of a property list serialization out to a stream.

Deprecated

### Validating a Property List

func CFPropertyListIsValid(CFPropertyList!, CFPropertyListFormat) -> Bool

Determines if a property list is valid.

### Data Types

struct CFPropertyListMutabilityOptions

Type for flags that determine the degree of mutability of newly created property lists.

### Constants

enum CFPropertyListFormat

Specifies the format of a property list.

Property List Mutability Options

Option flags that determine the degree of mutability of newly created property lists.

Reading and Writing Error Codes

Error codes for property list reading and writing functions such as CFPropertyListCreateWithData(_:_:_:_:_:).

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

XML Programming Topics for Core Foundation

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

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

