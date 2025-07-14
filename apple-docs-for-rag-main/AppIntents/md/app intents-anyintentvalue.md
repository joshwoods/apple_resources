

- App Intents
-  AnyIntentValue 

Protocol

# AnyIntentValue

A type the system uses to access a parameter or property value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol AnyIntentValue : Sendable
```

## Topics

### Getting the value type

associatedtype Value : _IntentValue, Sendable

**Required**

### Getting type-specific information

var title: LocalizedStringResource

**Required**

var isOptional: Bool

**Required**

## Relationships

### Inherits From

- Sendable

### Conforming Types

- EntityProperty
- IntentParameter

  Conforms when `Value` conforms to `_IntentValue` and `Sendable`.

- IntentParameterContext

## See Also

### Entity content

class EntityProperty

A property wrapper that exposes the associated property to the system.

protocol AppValue

An interface that describes conceptual types you use in app intents.

protocol AppEnum

An interface to express that a custom type has a predefined, static set of valid values to display.

protocol URLRepresentableEnum

An app enum with a URL representation.

