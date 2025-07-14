

- App Intents
-  StaticDisplayRepresentable 

Protocol

# StaticDisplayRepresentable

An interface for providing a static visual representation of a specific type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol StaticDisplayRepresentable : CaseDisplayRepresentable, TypeDisplayRepresentable
```

## Relationships

### Inherits From

- CaseDisplayRepresentable
- CaseIterable
- CustomLocalizedStringResourceConvertible
- Equatable
- Hashable
- TypeDisplayRepresentable

### Inherited By

- AppEnum
- AssistantEnum
- AssistantSchemaEnum
- URLRepresentableEnum

### Conforming Types

- StringSearchScope
- VideoCategory

## See Also

### Entity presentation

struct DisplayRepresentation

A type that describes the user interface presentation of a custom type.

protocol DisplayRepresentable

An interface for providing a dynamic visual representation of a specific type and instances of that type.

protocol InstanceDisplayRepresentable

An interface for providing the visual representation for an instance of a specific type.

protocol TypeDisplayRepresentable

An interface for providing the visual representation of a specific type.

struct TypeDisplayRepresentation

A type that describes the user interface presentation of a custom type.

protocol CaseDisplayRepresentable

An interface for providing the visual representation for an iterable collection of values.

