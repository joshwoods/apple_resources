

- App Intents
- IntentParameter
-  IntentParameter.PlacemarkDisplayStyle 

Enumeration

# IntentParameter.PlacemarkDisplayStyle

Describes a location’s display style in Shortcuts and Siri Suggestions.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum PlacemarkDisplayStyle
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Topics

### Getting the display styles

case name

A display style that shows only the location’s city.

case address

A display style that shows the location’s full address.

case city

A display style that shows only the location’s city.

### Operators

static func == (IntentParameter&lt;Value>.PlacemarkDisplayStyle, IntentParameter&lt;Value>.PlacemarkDisplayStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Accessing the display style

var displayStyle: IntentParameter&lt;Value>.PlacemarkDisplayStyle?

