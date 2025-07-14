

- Core Foundation
-  CFDate 

Class

# CFDate

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFDate
```

## Overview

`CFDate` objects store dates and times that can be compared to other dates and times. `CFDate` objects are immutable—there is no mutable counterpart for this opaque type.

`CFDate` provides functions for creating dates, comparing dates, and computing intervals. You use the CFDateCreate(_:_:) function to create `CFDate` objects. You use the CFDateCompare(_:_:_:) function to compare two dates, and the CFDateGetTimeIntervalSinceDate(_:_:) function to compute a time interval. Additional functions for managing dates and times are described in Time Utilities

`CFDate` is “toll-free bridged” with its Cocoa Foundation counterpart, NSDate. What this means is that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. In other words, in a method where you see an `NSDate *` parameter, you can pass in a `CFDateRef`, and in a function where you see a `CFDateRef` parameter, you can pass in an `NSDate` instance. This also applies to concrete subclasses of `NSDate`. See Interchangeable Data Types for more information on toll-free bridging.

## Topics

### CFDate Miscellaneous Functions

func CFDateCompare(CFDate!, CFDate!, UnsafeMutableRawPointer!) -> CFComparisonResult

Compares two `CFDate` objects and returns a comparison result.

func CFDateCreate(CFAllocator!, CFAbsoluteTime) -> CFDate!

Creates a `CFDate` object given an absolute time.

func CFDateGetAbsoluteTime(CFDate!) -> CFAbsoluteTime

Returns a `CFDate` object’s absolute time.

func CFDateGetTimeIntervalSinceDate(CFDate!, CFDate!) -> CFTimeInterval

Returns the number of elapsed seconds between the given `CFDate` objects.

func CFDateGetTypeID() -> CFTypeID

Returns the type identifier for the `CFDate` opaque type.

## Relationships

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

Date and Time Programming Guide for Core Foundation

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

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

