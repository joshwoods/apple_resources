

- Foundation
- Locale
- Locale.Language
-  hasCommonParent(with:) 

Instance Method

# hasCommonParent(with:)

Returns a Boolean value that indicates if the given language shares a common parent with this language.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func hasCommonParent(with language: Locale.Language) -> Bool
```

## Parameters 

`language`  

A language to compare parentage with.

## Return Value

`true` if this language and language share a common parent; `false` otherwise.

## See Also

### Examining language relationships

var parent: Locale.Language?

The parent language of this language, if available.

func isEquivalent(to: Locale.Language) -> Bool

Returns a Boolean value that indicates whether this language and another language are equivalent after expanding missing components.

