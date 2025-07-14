

- Foundation
- TermOfAddress
-  language 

Instance Property

# language

The specific language associated with a term of address.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var language: Locale.Language? { get }
```

## Discussion

This property is only set for terms of address created through the localized(language:pronouns:) function. This property is `nil` otherwise.

