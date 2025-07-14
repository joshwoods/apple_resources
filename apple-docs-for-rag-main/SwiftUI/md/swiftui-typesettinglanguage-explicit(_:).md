

- SwiftUI
- TypesettingLanguage
-  explicit(\_:) 

Type Method

# explicit(\_:)

Use explicit language.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func explicit(_ language: Locale.Language) -> TypesettingLanguage
```

## Parameters 

`language`  

The language to use for typesetting.

## Return Value

A `TypesettingLanguage`.

## Discussion

An explicit language will be used for typesetting. For example, if used with Thai language the line heights will be as tall as needed to accommodate Thai.

## See Also

### Getting language behavior

static let automatic: TypesettingLanguage

Automatic language behavior.

