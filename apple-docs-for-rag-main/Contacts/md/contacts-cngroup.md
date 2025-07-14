

- Contacts
-  CNGroup 

Class

# CNGroup

An immutable object that represents a group of contacts.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNGroup
```

## Overview

Contacts may be members of one or more groups, depending upon their accounts.

`CNGroup` objects are thread-safe, and you may access their properties from any thread of your app.

## Topics

### Getting the Group Information

var name: String

The name of the group.

var identifier: String

The unique identifier for a group on the device.

### Generating Search Predicates for Groups

The predicates to match groups. You can only use these predicates with CNGroup.

class func predicateForGroups(withIdentifiers: [String]) -> NSPredicate

Returns a predicate to find groups with the specified identifiers.

class func predicateForGroupsInContainer(withIdentifier: String) -> NSPredicate

Returns a predicate to find groups in the specified container.

class func predicateForSubgroupsInGroup(withIdentifier: String) -> NSPredicate

Returns a predicate to find subgroups in the specified parent group.

### Getting Group-Related Keys

let CNGroupIdentifierKey: String

The identifier of the group.

let CNGroupNameKey: String

The name of the group.

## Relationships

### Inherits From

- NSObject

### Inherited By

- CNMutableGroup

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSMutableCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Groups and Containers

class CNMutableGroup

A mutable object that represents a group of contacts.

class CNContainer

An immutable object that represents a collection of contacts.

