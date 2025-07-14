

- App Intents
- IntentPerson
- IntentPerson.Handle
-  IntentPerson.Handle.Label 

Enumeration

# IntentPerson.Handle.Label

A location description that applies to the handle’s content, for example a work or home phone number.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Label
```

## Topics

### Getting the handle labels

case home

case homeFax

case iPhone

case main

case mobile

case other

case pager

case school

case work

case workFax

### Operators

static func == (IntentPerson.Handle.Label, IntentPerson.Handle.Label) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case custom(String)

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

