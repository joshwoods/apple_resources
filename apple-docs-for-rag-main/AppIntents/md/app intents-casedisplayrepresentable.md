

- App Intents
-  CaseDisplayRepresentable 

Protocol

# CaseDisplayRepresentable

An interface for providing the visual representation for an iterable collection of values.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol CaseDisplayRepresentable : CustomLocalizedStringResourceConvertible, CaseIterable, Hashable
```

## Topics

### Describing the case conditions

static var caseDisplayRepresentations: [Self : DisplayRepresentation]

A dictionary that maps each value to the visual elements that represent it.

**Required**

### Providing a localized description

var localizedStringResource: LocalizedStringResource

var localizedStringResource: LocalizedStringResource

## Relationships

### Inherits From

- CaseIterable
- CustomLocalizedStringResourceConvertible
- Equatable
- Hashable

### Inherited By

- AppEnum
- AssistantEnum
- AssistantSchemaEnum
- StaticDisplayRepresentable
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

protocol StaticDisplayRepresentable

An interface for providing a static visual representation of a specific type.

