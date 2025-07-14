

- Core Spotlight
-  CSCustomAttributeKey 

Class

# CSCustomAttributeKey

A key associated with a custom attribute for a searchable item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+

``` source
class CSCustomAttributeKey
```

## Overview

The `CSCustomAttributeKey` class defines a key that you can associate with a custom attribute for a searchable item. Item attributes provide metadata about the item that can be indexed and displayed to users in search results.

Although the Core Spotlight framework provides several predefined attributes, such as title and description, you can create a `CSCustomAttributeKey` object to specify a custom attribute that makes sense in your domain.

## Topics

### Creating a custom attribute

convenience init?(keyName: String)

Returns a new custom attribute key with the specified name.

init?(keyName: String, searchable: Bool, searchableByDefault: Bool, unique: Bool, multiValued: Bool)

Returns a new custom attribute key with the specified name and properties.

### Getting the attribute details

var keyName: String

The name of the custom attribute key.

var isMultiValued: Bool

A Boolean value that indicates if the custom attribute is likely to have multiple values, such as arrays, associated with it.

var isSearchable: Bool

A Boolean value that indicates if the custom attribute can be specified as a search term.

var isSearchableByDefault: Bool

A Boolean value that indicates if the custom attribute should be searchable by default.

var isUnique: Bool

A Boolean value that indicates if duplicate custom attribute values should be treated as the same value to save storage space.

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

class CSLocalizedString

An object that displays localized text in search results related to your app.

class CSPerson

An object that represents a person in the context of search results.

