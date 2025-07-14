

- Foundation
-  NSException 

Class

# NSException

An object that represents a special condition that interrupts the normal flow of program execution.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSException
```

## Overview

Use NSException to implement exception handling. An exception is a special condition that interrupts the normal flow of program execution. Each application can interrupt the program for different reasons. For example, one application might interpret saving a file in a directory that is write-protected as an exception. In this sense, the exception is equivalent to an error. Another application might interpret the user’s key-press (for example, Control-C) as an exception: an indication that a long-running process should abort.

## Topics

### Creating and Raising an NSException Object

class func raise(NSExceptionName, format: String, arguments: CVaListPointer)

Creates and raises an exception with the specified name, reason, and arguments.

init(name: NSExceptionName, reason: String?, userInfo: [AnyHashable : Any]?)

Initializes and returns a newly allocated exception object.

func raise()

Raises the receiver, causing program flow to jump to the local exception handler.

### Querying an NSException Object

var name: NSExceptionName

A string used to uniquely identify the receiver.

var reason: String?

A string containing a “human-readable” reason for the receiver.

var userInfo: [AnyHashable : Any]?

A dictionary containing application-specific data pertaining to the receiver.

### Getting Exception Stack Frames

var callStackReturnAddresses: [NSNumber]

The call return addresses related to a raised exception.

var callStackSymbols: [String]

An array containing the current call stack symbols.

### Related Types

typealias NSUncaughtExceptionHandler

struct NSExceptionName

### Functions

func NSGetUncaughtExceptionHandler() -> ((NSException) -> Void)?

Returns the top-level error handler.

func NSSetUncaughtExceptionHandler(((NSException) -> Void)?)

Changes the top-level error handler.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

