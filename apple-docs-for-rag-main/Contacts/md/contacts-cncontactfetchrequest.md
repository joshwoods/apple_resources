

- Contacts
-  CNContactFetchRequest 

Class

# CNContactFetchRequest

An object that defines the options to use when fetching contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNContactFetchRequest
```

## Overview

You need at least one contact property key to fetch a contact’s properties. Use this class with the enumerateContacts(with:usingBlock:) method to execute the contact fetch request.

## Topics

### Creating a Fetch Request

init(keysToFetch: [any CNKeyDescriptor])

Creates a fetch request for the specified keys.

protocol CNKeyDescriptor

This protocol is reserved for Contacts framework usage.

### Specifying the Search Predicate

var predicate: NSPredicate?

The predicate to match contacts against.

### Configuring the Fetch Options

var mutableObjects: Bool

A Boolean value that indicates whether to return mutable contacts.

var unifyResults: Bool

A Boolean value that indicates whether to return linked contacts as unified contacts.

var sortOrder: CNContactSortOrder

The sort order for contacts.

enum CNContactSortOrder

Indicates the sorting order for contacts.

### Specifying the Keys to Fetch

var keysToFetch: [any CNKeyDescriptor]

The properties to fetch in the returned contacts.

## Relationships

### Inherits From

- CNFetchRequest

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Fetch and save requests

class CNFetchRequest

The base class for contact fetch requests.

class CNFetchResult

An object that represents the result of a change-history fetch request.

class CNSaveRequest

An object that collects the changes you want to save to the user’s contacts database.

