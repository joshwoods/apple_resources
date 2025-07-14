

- CallKit
-  CXCallDirectoryExtensionContext 

Class

# CXCallDirectoryExtensionContext

A programmatic interface for adding identification and blocking entries to a Call Directory app extension.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
class CXCallDirectoryExtensionContext
```

## Overview

The system doesn’t initialize CXCallDirectoryExtensionContext objects directly, but instead passes them as arguments to the CXCallDirectoryProvider instance method beginRequest(with:).

## Topics

### Setting the Delegate

var delegate: (any CXCallDirectoryExtensionContextDelegate)?

Sets a delegate that can handle request failures for the Call Directory extension context object.

### Adding Entries

func addIdentificationEntry(withNextSequentialPhoneNumber: CXCallDirectoryPhoneNumber, label: String)

Adds an identification entry with the specified phone number and label.

func addBlockingEntry(withNextSequentialPhoneNumber: CXCallDirectoryPhoneNumber)

Adds a blocking entry with the specified phone number.

### Removing Entries

func removeAllBlockingEntries()

Removes all stored blocking entries.

func removeAllIdentificationEntries()

Removes all stored identification entries.

func removeBlockingEntry(withPhoneNumber: CXCallDirectoryPhoneNumber)

Removes a blocking entry that contains the specified phone number.

func removeIdentificationEntry(withPhoneNumber: CXCallDirectoryPhoneNumber)

Removes an identification entry that contains the specified phone number.

### Completing Requests

var isIncremental: Bool

A Boolean value that indicates whether the request provides data incrementally.

func completeRequest(completionHandler: ((Bool) -> Void)?)

Completes the request to the extension context.

### Types

typealias CXCallDirectoryPhoneNumber

A value that represents a phone number consisting of a country calling code followed by a sequence of digits.

let CXCallDirectoryPhoneNumberMax: CXCallDirectoryPhoneNumber

The maximum allowable value for a phone number.

## Relationships

### Inherits From

- NSExtensionContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Caller ID

Identifying and blocking calls

Create a Call Directory app extension to identify and block incoming callers by their phone number.

class CXCallDirectoryProvider

The principal object for a Call Directory app extension for a host app.

protocol CXCallDirectoryExtensionContextDelegate

A collection of methods a Call Directory extension context object calls when a request fails.

class CXCallDirectoryManager

The programmatic interface to an object that manages a Call Directory app extension.

