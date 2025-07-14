

- App Intents
-  AppEnum 

Protocol

# AppEnum

An interface to express that a custom type has a predefined, static set of valid values to display.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
protocol AppEnum : AppValue, StaticDisplayRepresentable, RawRepresentable where Self.RawValue : LosslessStringConvertible
```

## Mentioned in 

Integrating actions with Siri and Apple Intelligence

Integrating custom data types into your intents

Adding parameters to an app intent

Responding to the Action button on Apple Watch Ultra

## Overview

Adopt the AppEnum protocol in a type that has a known set of valid values. You might use this protocol to specify that a variable of one of your intents has a fixed set of possible values. For example, you might use a variable to specify whether to navigate to the next or previous track in a music playlist.

Because this type conforms to the StaticDisplayRepresentable protocol, provide a string-based representation of your type’s values in your implementation. For example, provide descriptions for each case of an `enum` type in the inherited caseDisplayRepresentations property.

## Topics

### Resolving the type

static var defaultResolverSpecification: some ResolverSpecification

## Relationships

### Inherits From

- AppValue
- CaseDisplayRepresentable
- CaseIterable
- CustomLocalizedStringResourceConvertible
- Equatable
- Hashable
- PersistentlyIdentifiable
- RawRepresentable
- Sendable
- StaticDisplayRepresentable
- TypeDisplayRepresentable

### Inherited By

- AssistantEnum
- AssistantSchemaEnum
- URLRepresentableEnum

### Conforming Types

- StringSearchScope
- VideoCategory

## See Also

### Entity content

class EntityProperty

A property wrapper that exposes the associated property to the system.

protocol AppValue

An interface that describes conceptual types you use in app intents.

protocol AnyIntentValue

A type the system uses to access a parameter or property value.

protocol URLRepresentableEnum

An app enum with a URL representation.

