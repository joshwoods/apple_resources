

- Foundation
- Locale
- Locale.Language
-  isEquivalent(to:) 

Instance Method

# isEquivalent(to:)

Returns a Boolean value that indicates whether this language and another language are equivalent after expanding missing components.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func isEquivalent(to language: Locale.Language) -> Bool
```

## Parameters 

`language`  

A language to compare equivalence with.

## Return Value

`true` if the two languages are equivalent; `false` otherwise.

## Discussion

The following example shows equivalence tests run on various ways of expressing the US English language, followed by a test against UK English.

```
let en = Locale.Language(identifier: "en")
let enUS = Locale.Language(identifier: "en-US")
let enLatn = Locale.Language(identifier: "en-Latn")
let enLatnUS = Locale.Language(identifier: "en-Latn-US")

let test1 = en.isEquivalent(to: enUS) // true
let test2 = en.isEquivalent(to: enLatn) // true
let test3 = en.isEquivalent(to: enLatnUS) // true

let enUK = Locale.Language(identifier: "en-UK")
let test4 = en.isEquivalent(to: enUK) // false
```

## See Also

### Examining language relationships

var parent: Locale.Language?

The parent language of this language, if available.

func hasCommonParent(with: Locale.Language) -> Bool

Returns a Boolean value that indicates if the given language shares a common parent with this language.

