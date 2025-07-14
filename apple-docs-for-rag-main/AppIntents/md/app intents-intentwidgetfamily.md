

- App Intents
-  IntentWidgetFamily 

Enumeration

# IntentWidgetFamily

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+watchOS 10.0+

``` source
enum IntentWidgetFamily
```

## Topics

### Operators

static func == (IntentWidgetFamily, IntentWidgetFamily) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case accessoryCircular

A circular widget.

case accessoryCorner

A corner widget.

case accessoryInline

A flat widget that contains a single row of text and an optional image.

case accessoryRectangular

A rectangular widget.

case systemExtraLarge

An extra large widget.

case systemLarge

A large widget.

case systemMedium

A medium-sized widget.

case systemSmall

A small widget.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias Specification

typealias UnwrappedType

typealias ValueType

### Type Properties

static var defaultResolverSpecification: EmptyResolverSpecification&lt;IntentWidgetFamily>

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

