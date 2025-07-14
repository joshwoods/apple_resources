

- App Intents
-  InstanceDisplayRepresentable 

Protocol

# InstanceDisplayRepresentable

An interface for providing the visual representation for an instance of a specific type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol InstanceDisplayRepresentable : CustomLocalizedStringResourceConvertible
```

## Topics

### Providing the visual content

var displayRepresentation: DisplayRepresentation

The visual elements to display when presenting an instance of the type.

**Required** Default implementations provided.

### Providing a localized description

var localizedStringResource: LocalizedStringResource

## Relationships

### Inherits From

- CustomLocalizedStringResourceConvertible

### Inherited By

- AppEntity
- AssistantEntity
- AssistantSchemaEntity
- DisplayRepresentable
- FileEntity
- IndexedEntity
- SetFocusFilterIntent
- StartWorkoutIntent
- TransientAppEntity
- URLRepresentableEntity
- UniqueAppEntity

### Conforming Types

- IntentCurrencyAmount
- IntentFile
- IntentPaymentMethod
- IntentPerson

## See Also

### Entity presentation

struct DisplayRepresentation

A type that describes the user interface presentation of a custom type.

protocol DisplayRepresentable

An interface for providing a dynamic visual representation of a specific type and instances of that type.

protocol TypeDisplayRepresentable

An interface for providing the visual representation of a specific type.

struct TypeDisplayRepresentation

A type that describes the user interface presentation of a custom type.

protocol StaticDisplayRepresentable

An interface for providing a static visual representation of a specific type.

protocol CaseDisplayRepresentable

An interface for providing the visual representation for an iterable collection of values.

