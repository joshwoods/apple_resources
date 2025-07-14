

- Foundation
- Locale
- Locale.Language
-  parent 

Instance Property

# parent

The parent language of this language, if available.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var parent: Locale.Language? { get }
```

## Discussion

For example, the parent language of `en_US_POSIX` is `en_US`.

If the system can’t determine a parent language, this value is `nil`.

## See Also

### Examining language relationships

func hasCommonParent(with: Locale.Language) -> Bool

Returns a Boolean value that indicates if the given language shares a common parent with this language.

func isEquivalent(to: Locale.Language) -> Bool

Returns a Boolean value that indicates whether this language and another language are equivalent after expanding missing components.

