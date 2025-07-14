

- Core Foundation
-  CFError 

Class

# CFError

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFError
```

## Overview

A CFError object encapsulates more rich and extensible error information than is possible using only an error code or error string. The core attributes of a CFError object are an error domain (represented by a string), a domain-specific error code, and a “user info” dictionary containing application-specific information. Errors are required to have a domain and an error code within that domain. Several well-known domains are defined corresponding to Mach, POSIX, and OSStatus errors.

The optional “user info” dictionary may provide additional information that might be useful for the interpretation and reporting of the error, including a human-readable description for the error. The “user info” dictionary sometimes includes another CFError object that represents an error in a subsystem underlying the error represented by the containing CFError object. This underlying error object may provide more specific information about the cause of the error.

In general, a method should signal an error condition by returning, for example, `false` or `NULL` rather than by the simple presence of an error object. The method can then optionally return an CFError object by reference, in order to further describe the error.

CFError is toll-free bridged to NSError in the Foundation framework—for more details on toll-free bridging, see Toll-Free Bridged Types. `NSError` has some additional guidelines that make it easy to report errors automatically to users and attempt to recover from them. See Error Handling Programming Guide for more information on `NSError` programming guidelines.

## Topics

### Creating a CFError

func CFErrorCreate(CFAllocator!, CFErrorDomain!, CFIndex, CFDictionary!) -> CFError!

Creates a new CFError object.

func CFErrorCreateWithUserInfoKeysAndValues(CFAllocator!, CFErrorDomain!, CFIndex, UnsafePointer&lt;UnsafeRawPointer?>!, UnsafePointer&lt;UnsafeRawPointer?>!, CFIndex) -> CFError!

Creates a new CFError object using given keys and values to create the user info dictionary.

### Getting Information About an Error

func CFErrorGetDomain(CFError!) -> CFErrorDomain!

Returns the error domain for a given CFError.

func CFErrorGetCode(CFError!) -> CFIndex

Returns the error code for a given CFError.

func CFErrorCopyUserInfo(CFError!) -> CFDictionary!

Returns the user info dictionary for a given CFError.

func CFErrorCopyDescription(CFError!) -> CFString!

Returns a human-presentable description for a given error.

func CFErrorCopyFailureReason(CFError!) -> CFString!

Returns a human-presentable failure reason for a given error.

func CFErrorCopyRecoverySuggestion(CFError!) -> CFString!

Returns a human presentable recovery suggestion for a given error.

### Getting the CFError Type ID

func CFErrorGetTypeID() -> CFTypeID

Returns the type identifier for the CFError opaque type.

### Constants

Error domains

These constants define domains for CFError objects.

Keys for the user info dictionary

Keys in the `userInfo` dictionary.

## Relationships

### Conforms To

- Copyable
- Equatable
- Error
- Hashable
- Sendable

## See Also

### Related Documentation

Error Handling Programming Guide

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

class CFFileDescriptor

