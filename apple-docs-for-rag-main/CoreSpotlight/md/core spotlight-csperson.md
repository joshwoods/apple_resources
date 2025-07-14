

- Core Spotlight
-  CSPerson 

Class

# CSPerson

An object that represents a person in the context of search results.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class CSPerson
```

## Overview

A `CSPerson` object represents a person in the context of search results. You can create a `CSPerson` object when you have a display name and a contact handle of some kind, such as an email address or phone number.

If you create a `CSPerson` object to represent a specific contact, you can use the value of the contact’s identifier property for the person object’s contactIdentifier property. Using the same value lets you avoid using names or phone numbers to look up the contact that’s associated with a person.

## Topics

### Initializing a person object

init(displayName: String?, handles: [String], handleIdentifier: String)

Returns a new `CSPerson` object initialized with the specified display name and contact attributes.

### Accessing person properties

var contactIdentifier: String?

The identifier for the contact associated with the person.

var displayName: String?

A display name for the person.

var handleIdentifier: String

A key that identifies the type of contact property represented by the person object’s handle.

var handles: [String]

An array of contact handles related to the person.

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

### Searchable items

class CSSearchableItem

The details of your app-specific content that someone might search for on their devices.

class CSSearchableItemAttributeSet

The detailed metadata for a searchable item.

class CSCustomAttributeKey

A key associated with a custom attribute for a searchable item.

class CSLocalizedString

An object that displays localized text in search results related to your app.

