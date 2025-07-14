

- Foundation
- InflectionConcept
-  InflectionConcept.termsOfAddress(\_:) 

Case

# InflectionConcept.termsOfAddress(\_:)

Indicates that the system uses the associated terms of address for grammatical agreement when localizing text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
case termsOfAddress([TermOfAddress])
```

## Parameters 

`[TermOfAddress]`  

A list of preferred terms of address for localizing text.

## Discussion

When inflecting text the first term of address which can be used in the target language is the one used for pronoun substitution and grammar agreement.

## See Also

### Using inflection concepts

case localizedPhrase(String)

Indicates that the system uses the associated string for grammatical agreement when localizing text.

