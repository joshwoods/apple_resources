

- Foundation
- InflectionRule
-  canInflect(language:) 

Type Method

# canInflect(language:)

Returns a Boolean value that indicates whether the rule can inflect a given language.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func canInflect(language: String) -> Bool
```

## Parameters 

`language`  

The language to apply inflection to, specified as a BCP 47 language code.

## Return Value

`true` if the rule can inflect the given language; otherwise, `false`.

## See Also

### Determining Availability

static var canInflectPreferredLocalization: Bool

A Boolean value that indicates whether the rule can inflect the user’s current preferred localization.

