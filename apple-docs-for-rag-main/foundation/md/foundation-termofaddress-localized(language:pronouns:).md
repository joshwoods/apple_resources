

- Foundation
- TermOfAddress
-  localized(language:pronouns:) 

Type Method

# localized(language:pronouns:)

Returns a term of address restricted to a specific language for a group of pronouns.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func localized(
    language: Locale.Language,
    pronouns: [Morphology.Pronoun]
) -> TermOfAddress
```

## Parameters 

`language`  

The language locale to use for the term of address.

`pronouns`  

The pronouns for representing the terms of address.

## Return Value

A term of address associating a group of pronouns to a specific language.

