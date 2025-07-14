

- Contacts
-  CNContainer 

Class

# CNContainer

An immutable object that represents a collection of contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNContainer
```

## Overview

A contact can be in only one container. CardDAV accounts usually have only one container whereas Exchange accounts may have multiple containers, where each container represents an Exchange folder.

`CNContainer` objects are thread-safe, and you may access their properties from any thread of your app.

## Topics

### Getting the Container Information

var name: String

The name of the container.

var identifier: String

The unique identifier for a contacts container on the device.

var type: CNContainerType

The type of the container.

enum CNContainerType

The container may be local on the device or associated with a server account that has contacts.

### Generating Search Predicates for Containers

These are the predicates to match containers contacts. You can only use these predicates with `CNContainer`.

class func predicateForContainerOfContact(withIdentifier: String) -> NSPredicate

Returns a predicate to find the container of the specified contact.

class func predicateForContainers(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find the containers with the specified identifiers.

class func predicateForContainerOfGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find the container of the specified group.

### Getting Container-Related Keys

let CNContainerIdentifierKey: String

The identifier key of the container.

let CNContainerNameKey: String

The name of the container.

let CNContainerTypeKey: String

The type of the container.

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

## See Also

### Groups and Containers

class CNGroup

An immutable object that represents a group of contacts.

class CNMutableGroup

A mutable object that represents a group of contacts.

