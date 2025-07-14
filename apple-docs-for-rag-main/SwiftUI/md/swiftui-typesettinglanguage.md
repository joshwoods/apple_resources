

- SwiftUI
-  TypesettingLanguage 

Structure

# TypesettingLanguage

Defines how typesetting language is determined for text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct TypesettingLanguage
```

## Overview

Use a modifier like typesettingLanguage(_:isEnabled:) to specify the typesetting language.

## Topics

### Getting language behavior

static let automatic: TypesettingLanguage

Automatic language behavior.

static func explicit(Locale.Language) -> TypesettingLanguage

Use explicit language.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Localizing text

Preparing views for localization

Specify hints and add strings to localize your SwiftUI views.

struct LocalizedStringKey

The key used to look up an entry in a strings file or strings dictionary file.

var locale: Locale

The current locale that views should use.

func typesettingLanguage(_:isEnabled:)

Specifies the language for typesetting.

