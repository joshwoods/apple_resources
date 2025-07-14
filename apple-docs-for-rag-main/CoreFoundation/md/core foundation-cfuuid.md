

- Core Foundation
-  CFUUID 

Class

# CFUUID

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFUUID
```

## Overview

CFUUID objects are used by plug-ins to uniquely identify types, interfaces, and factories. When creating a new type, host developers must generate UUIDs to identify the type as well as its interfaces and factories.

UUIDs (Universally Unique Identifiers), also known as GUIDs (Globally Unique Identifiers) or IIDs (Interface Identifiers), are 128-bit values designed to be unique.

The standard format for UUIDs represented in ASCII is a string punctuated by hyphens, for example `68753A44-4D6F-1226-9C60-0050E4C00067`. The hex representation looks, as you might expect, like a list of numerical values preceded by `0x`. For example, `0x68, 0x75, 0x3A, 0x44, 0x4D, 0x6F, 0x12, 0x26, 0x9C, 0x60, 0x00, 0x50, 0xE4, 0xC0, 0x00, 0x67` . To use a UUID, you create it and then copy the resulting strings into your header and C language source files. Because a UUID is expressed as an array of bytes, there are no endianness considerations for different platforms.

You can create a CFUUID object using any one of the `CFUUIDCreate...` functions. Use the CFUUIDGetConstantUUIDWithBytes(_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:_:) function if you want to declare a UUID constant in a `#define` statement. You can get the raw bytes of an existing CFUUID object using the CFUUIDGetUUIDBytes(_:) function.

## Topics

### Creating CFUUID Objects

func CFUUIDCreate(CFAllocator!) -> CFUUID!

Creates a Universally Unique Identifier (UUID) object.

func CFUUIDCreateFromString(CFAllocator!, CFString!) -> CFUUID!

Creates a CFUUID object for a specified string.

func CFUUIDCreateFromUUIDBytes(CFAllocator!, CFUUIDBytes) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

func CFUUIDCreateWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Creates a CFUUID object from raw UUID bytes.

### Getting Information About CFUUID Objects

func CFUUIDCreateString(CFAllocator!, CFUUID!) -> CFString!

Returns the string representation of a specified CFUUID object.

func CFUUIDGetConstantUUIDWithBytes(CFAllocator!, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8, UInt8) -> CFUUID!

Returns a CFUUID object from raw UUID bytes.

func CFUUIDGetUUIDBytes(CFUUID!) -> CFUUIDBytes

Returns the value of a UUID object as raw bytes.

### Getting the CFUUID Type Identifier

func CFUUIDGetTypeID() -> CFTypeID

Returns the type identifier for all CFUUID objects.

### Data Types

struct CFUUIDBytes

A 128-bit struct that represents a UUID as raw bytes.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

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

