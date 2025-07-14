

- App Intents
-  URLRepresentableEnum 

Protocol

# URLRepresentableEnum

An app enum with a URL representation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
protocol URLRepresentableEnum : AppEnum, CustomURLRepresentationParameterConvertible
```

## Overview

Add support for `URLRepresentableEnum` to your app enums to add a URL representation. This allows Siri and Shortcuts to treat the enum like a universal link to specific content, allowing actions to open the URL or to make it sharable.

Note that you need to use a universal link for your URL representation, you can’t use a custom URL scheme. For more information about universal links, see Allowing apps and websites to link to your content.

## Topics

### Type Aliases

typealias URLRepresentation

### Type Properties

static var urlRepresentation: Self.URLRepresentation

**Required** Default implementation provided.

## Relationships

### Inherits From

- AppEnum
- AppValue
- CaseDisplayRepresentable
- CaseIterable
- CustomLocalizedStringResourceConvertible
- CustomURLRepresentationParameterConvertible
- Equatable
- Hashable
- PersistentlyIdentifiable
- RawRepresentable
- Sendable
- StaticDisplayRepresentable
- TypeDisplayRepresentable

## See Also

### Entity content

class EntityProperty

A property wrapper that exposes the associated property to the system.

protocol AppValue

An interface that describes conceptual types you use in app intents.

protocol AnyIntentValue

A type the system uses to access a parameter or property value.

protocol AppEnum

An interface to express that a custom type has a predefined, static set of valid values to display.

