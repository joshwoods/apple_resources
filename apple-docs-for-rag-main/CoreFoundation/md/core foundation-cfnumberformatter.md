

- Core Foundation
-  CFNumberFormatter 

Class

# CFNumberFormatter

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFNumberFormatter
```

## Overview

CFNumberFormatter objects format the textual representations of CFNumber objects, and convert textual representations of numbers into CFNumber objects. The representation encompasses integers, floats, and doubles; floats and doubles can be formatted to a specified decimal position. You specify how strings are formatted and parsed by setting a format string and other properties of a CFNumberFormatter object.

The format of the format string is defined by Unicode Technical Standard \#35; the version of the standard used varies with release of the operating system, and is described in Introduction to Data Formatting Programming Guide For Cocoa.

Important

`CFNumberFormatter` is not thread-safe. Do not use a single instance from multiple threads.

Unlike some other Core Foundation opaque types with names similar to a corresponding Cocoa Foundation class (such as CFString and `NSString`), CFNumberFormatter objects cannot be cast (“toll-free bridged”) to `NSNumberFormatter` objects.

## Topics

### Creating a Number Formatter

func CFNumberFormatterCreate(CFAllocator!, CFLocale!, CFNumberFormatterStyle) -> CFNumberFormatter!

Creates a new CFNumberFormatter object, localized to the given locale, which will format numbers to the given style.

### Configuring a Number Formatter

func CFNumberFormatterSetFormat(CFNumberFormatter!, CFString!)

Sets the format string of a number formatter.

func CFNumberFormatterSetProperty(CFNumberFormatter!, CFNumberFormatterKey!, CFTypeRef!)

Sets a number formatter property using a key-value pair.

### Formatting Values

func CFNumberFormatterCreateNumberFromString(CFAllocator!, CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFOptionFlags) -> CFNumber!

Returns a number object representing a given string.

func CFNumberFormatterCreateStringWithNumber(CFAllocator!, CFNumberFormatter!, CFNumber!) -> CFString!

Returns a string representation of the given number using the specified number formatter.

func CFNumberFormatterCreateStringWithValue(CFAllocator!, CFNumberFormatter!, CFNumberType, UnsafeRawPointer!) -> CFString!

Returns a string representation of the given number or value using the specified number formatter.

func CFNumberFormatterGetDecimalInfoForCurrencyCode(CFString!, UnsafeMutablePointer&lt;Int32>!, UnsafeMutablePointer&lt;Double>!) -> Bool

Returns the number of fraction digits that should be displayed, and the rounding increment, for a given currency.

func CFNumberFormatterGetValueFromString(CFNumberFormatter!, CFString!, UnsafeMutablePointer&lt;CFRange>!, CFNumberType, UnsafeMutableRawPointer!) -> Bool

Returns a number or value representing a given string.

### Examining a Number Formatter

func CFNumberFormatterCopyProperty(CFNumberFormatter!, CFNumberFormatterKey!) -> CFTypeRef!

Returns a copy of a number formatter’s value for a given key.

func CFNumberFormatterGetFormat(CFNumberFormatter!) -> CFString!

Returns a format string for the given number formatter object.

func CFNumberFormatterGetLocale(CFNumberFormatter!) -> CFLocale!

Returns the locale object used to create the given number formatter object.

func CFNumberFormatterGetStyle(CFNumberFormatter!) -> CFNumberFormatterStyle

Returns the number style used to create the given number formatter object.

### Getting the CFNumberFormatter Type ID

func CFNumberFormatterGetTypeID() -> CFTypeID

Returns the type identifier for the `CFNumberFormatter` opaque type.

### Data Types

enum CFNumberFormatterStyle

Type for constants specifying a formatter style.

struct CFNumberFormatterOptionFlags

Type for constants specifying how numbers should be parsed.

enum CFNumberFormatterPadPosition

Type for constants specifying how numbers should be padded.

### Constants

Number Formatter Styles

Predefined number format styles.

Number Formatter Property Keys

The keys used in key-value pairs to specify the value of number formatter properties.

Number Format Options

These constants are used to specify how numbers should be parsed.

enum CFNumberFormatterRoundingMode

These constants are used to specify how numbers should be rounded.

Padding Positions

These constants are used to specify how numbers should be padded.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Data Formatting Guide for Core Foundation

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

