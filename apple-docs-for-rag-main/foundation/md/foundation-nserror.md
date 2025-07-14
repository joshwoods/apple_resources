

- Foundation
-  NSError 

Class

# NSError

Information about an error condition including a domain, a domain-specific error code, and application-specific information.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class NSError
```

## Overview

Objective-C methods can signal an error condition by returning an NSError object by reference, which provides additional information about the kind of error and any underlying cause, if one can be determined. An NSError object may also provide localized error descriptions suitable for display to the user in its user info dictionary. See Error Handling Programming Guide for more information.

Methods in Foundation and other Cocoa frameworks most often produce errors in the Cocoa error domain (NSCocoaErrorDomain); error codes for the Cocoa Error Domain are documented in the Foundation Constants. There are also predefined domains corresponding to Mach (NSMachErrorDomain), POSIX (NSPOSIXErrorDomain), and Carbon (NSOSStatusErrorDomain) errors.

NSError is “toll-free bridged” with its Core Foundation counterpart, CFError. See Toll-Free Bridging for more information.

### Subclassing Notes

Applications may choose to create subclasses of `NSError`, for example, to provide better localized error strings by overriding localizedDescription.

## Topics

### Creating Error Objects

init(domain: String, code: Int, userInfo: [String : Any]?)

Returns an `NSError` object initialized for a given domain and code with a given `userInfo` dictionary.

### Getting Error Properties

var code: Int

The error code.

var domain: String

A string containing the error domain.

var userInfo: [String : Any]

The user info dictionary.

### Getting a Localized Error Description

var localizedDescription: String

A string containing the localized description of the error.

var localizedRecoveryOptions: [String]?

An array containing the localized titles of buttons appropriate for displaying in an alert panel.

var localizedRecoverySuggestion: String?

A string containing the localized recovery suggestion for the error.

var localizedFailureReason: String?

A string containing the localized explanation of the reason for the error.

### Providing Error User Info

class func setUserInfoValueProvider(forDomain: String, provider: ((any Error, String) -> Any?)?)

Specifies a block to call when the corresponding property is not present in the user info dictionary.

class func userInfoValueProvider(forDomain: String) -> ((any Error, String) -> Any?)?

Returns any user info provider specified for a given error domain.

struct ErrorUserInfoKey

typealias UserInfoKey

These keys may exist in the user info dictionary.

### Getting the Error Recovery Attempter

var recoveryAttempter: Any?

The object in the user info dictionary corresponding to the NSRecoveryAttempterErrorKey key.

NSErrorRecoveryAttempting

A set of methods that provide options to recover from an error.

### Displaying a Help Anchor

var helpAnchor: String?

A string to display in response to an alert panel help anchor button being pressed.

### Supporting Types

typealias ErrorPointer

typealias NSErrorPointer

typealias NSErrorDomain

### Error Domains

let NSCocoaErrorDomain: String

Cocoa errors

let NSPOSIXErrorDomain: String

POSIX/BSD errors

let NSOSStatusErrorDomain: String

Mac OS 9/Carbon errors

let NSMachErrorDomain: String

Mach errors

let NSURLErrorDomain: String

URL loading system errors

let NSStreamSOCKSErrorDomain: String

The error domain used by `NSError` when reporting SOCKS errors.

let NSStreamSocketSSLErrorDomain: String

The error domain used by `NSError` when reporting SSL errors.

### Error Codes

struct CocoaError

Describes errors within the Cocoa error domain.

struct MachError

Describes an error in the Mach error domain.

struct POSIXError

Describes an error in the POSIX error domain.

NSError Codes

Error codes in the Cocoa error domain.

### Instance Properties

var underlyingErrors: [any Error]

### Type Methods

class func fileProviderErrorForCollision(with: NSFileProviderItem) -> Self

Returns a properly formatted error object with a `NSFileProviderItemCollisionError` error code.

class func fileProviderErrorForNonExistentItem(withIdentifier: NSFileProviderItemIdentifier) -> Self

class func fileProviderErrorForRejectedDeletion(of: NSFileProviderItem) -> Self

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Error
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### User-Relevant Errors

protocol Error : Sendable

A type representing an error value that can be thrown.

protocol LocalizedError

A specialized error that provides localized messages describing the error and why it occurred.

protocol RecoverableError

A specialized error that may be recoverable by presenting several potential recovery options to the user.

protocol CustomNSError

A specialized error that provides a domain, error code, and user-info dictionary.

