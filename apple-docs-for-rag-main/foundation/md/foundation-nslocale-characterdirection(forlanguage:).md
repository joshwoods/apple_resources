

- Foundation
- NSLocale
-  characterDirection(forLanguage:) 

Type Method

# characterDirection(forLanguage:)

Returns the direction of the sequence of characters in a line for the specified ISO language code.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func characterDirection(forLanguage isoLangCode: String) -> NSLocale.LanguageDirection
```

## Parameters 

`isoLangCode`  

The ISO language code.

## Return Value

Returns the direction in which characters appear within a line in the specified language. See NSLocale.LanguageDirection for possible values. If the appropriate direction can’t be determined NSLocale.LanguageDirection.unknown is returned.

## See Also

### Getting Line and Character Direction for a Language

class func lineDirection(forLanguage: String) -> NSLocale.LanguageDirection

Returns the direction of the sequence of lines for the specified ISO language code.

enum LanguageDirection

The directions that a language may take across a page of text.

