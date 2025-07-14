

- Foundation
- TermOfAddress
-  pronouns 

Instance Property

# pronouns

The pronouns associated with a term of address.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var pronouns: [Morphology.Pronoun] { get }
```

## Discussion

This property is only set for terms of address created through the localized(language:pronouns:) function. Calling this property returns an empty array otherwise.

