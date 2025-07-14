

- Contacts
-  CNContactRelation 

Class

# CNContactRelation

An immutable object that represents the relationship between one contact to another.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 2.0+

``` source
class CNContactRelation
```

## Overview

`CNContactRelation` objects are thread-safe, and you may access their properties from any thread of your app.

## Topics

### Creating a Contact Relation Object

init(name: String)

Creates an object with the name of the related contact.

### Getting the Relation Name

var name: String

The name of the related contact.

### Getting the Common Relationship Labels

let CNLabelContactRelationSpouse: String

The label for the contact’s spouse.

let CNLabelContactRelationPartner: String

The label for the contact’s partner.

let CNLabelContactRelationDaughter: String

The label for the contact’s daughter.

let CNLabelContactRelationSon: String

The label for the contact’s son.

let CNLabelContactRelationChild: String

The label for the contact’s child.

let CNLabelContactRelationFather: String

The label for the contact’s father.

let CNLabelContactRelationMother: String

The label for the contact’s mother.

let CNLabelContactRelationParent: String

The label for the contact’s parent.

let CNLabelContactRelationBrother: String

The label for the contact’s brother.

let CNLabelContactRelationSister: String

The label for the contact’s sister.

let CNLabelContactRelationFriend: String

The label for the contact’s friend.

let CNLabelContactRelationAssistant: String

The label for the contact’s assistant.

let CNLabelContactRelationManager: String

The label for the contact’s manager.

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

